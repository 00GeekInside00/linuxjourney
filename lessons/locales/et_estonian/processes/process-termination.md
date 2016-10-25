# Protsesside peatamine

## Tunni sisu

�ppisime, mis toimub, kui protsesse luuakse, kuid mis saab siis kui neid enam vaja pole? Ole hoiatatud, Linux kipub vahel veidi s�ngeks...

Protsessist v�ib v�ljuda kasutades *_exit* s�steemset kutset. Sellisel juhul vabastatakse protsessi ressursid �mberjaotamise tarbeks. Kui protsess on valmis oma t��d l�petama, annab ta tuumale teada l�petamise p�hjuse l�bi l�petamise staatuse. Tavaliselt t�hendab 0, et protsess oli edukas. Kuid sellest ei piisa, et protsessi t��d l�petada. Emaprotsess peab t�tre t�� l�petamist tunnistama kasutades selleks *wait* s�steemset kutset, mis kontrollib t�tarporsessi t�� peatamise seisundit. V�ib ju tunduda julm, aga *wait* kutse on paratamatult vajalik, sest milline ema ei tahaks teada, kuidas nende laps suri?

On veel �ks viis protsessi peatamiseks, mis h�lmab signaalide kasutamist, millest r��gitakse �igepea.

<b>H�ljatud protsessid</b>

Kui emaprotsess peaks surema enne kui t�tarprotsess, siis tuum teab, et *wai* kutset ei tule. Need protsessid nimetatakse orbudeks ja antakse *inti*i hoole alla (m�letatavasti k�ikide protsesside ema). *Init* teostab mingil hetkel ikkagi *wait* kutse, nii et need h�jatud protsessid saavad ka �ra l�ppeda.

<b>Zombiprotsessid</b>

Mis juhtub aga kui t�tar on peatunud aga emaprotsess pole veel *wait* kutset teostanud? Soovime sellegi poolest teada, kuidas see juhtus ning hoolimata sellest, et t�tarprotsess oma tegevuse l�petas, muudab tuum ta zombiprotsessiks. T�tarprotsessi ressursid on ikkagi vabastatud, kuid protsesside tabelis on selle zombi kohta endiselt kanne. Zombiprotsesse ei saa "tappa", st sunniviisiliselt peatada, kuna nad on juba tegelikult peatunud. Zombide tapmiseks kasutatakse signaale. Kui l�puks emaprotsess selle *wait* s�steemse kutse teostab, saab zombi kaduda, seda protsessi nimetatakse *reaping* (l�ikus). Kui ema *wait* kutset ei teoasta, lapsendab *init* selle zombi ja teeb seda automaatselt ise, mille j�rel zombi eemaldatakse. Zombide �lek�llus v�ib olla v�ga halb, kuna nad v�tavad tabelis ruumi ning seega ei v�imalda teistel protsessidel t��tada.

## Harjutus

Selles peat�kis harjutuse pole.

## K�simus

Milline on k�ige tavalisem edukalt t�� l�petanud protsessi peatumise staatus?

## Vastus

0
