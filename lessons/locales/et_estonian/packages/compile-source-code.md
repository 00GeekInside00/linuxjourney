# L�htekoodi kompileerimine

## Tunni sisu

Vahel v�ib sattuda m�ne sellise segase paketi otsa, mis on saadaval ainult puhtas l�htekoodis. Selleks, et seda kompileerida ja paigaldada on vaja teada paari k�sku.

Esiteks aga on vaja tarkvara, et paigaldada t��riistad, mis v�imaldaksid l�htekoodi kompileerida.

<pre>$ sudo apt install build-essential</pre>

Kui see on tehtud, on vaja paketi faili sisu lahti pakkida. See on ilmselt .tar.gz fail.

<pre>$ tar -xzvf pakett.tar.gz</pre>

Enne kui �ldse midagi tegema hakata, v�iks lugeda *README* v�i *INSTALL* faili paketis. M�nikord v�ib sealt leida paigaldamiseks spetsiifilisi juhiseid. 

Olenevalt sellest, milliseid kompileerimise meetodeid kasutas arendaja, v�ib vaja minna erinevaid k�ske, n�iteks *cmake* v�i midagi muud.

Tavalisemalt kasutatakse aga ikkagi *make* kompilatsiooni, seega r��gitakse just sellest l�hemalt:

Paketis asub konfiguratsiooni skript, mis kontrollib s�steemis s�ltuvusi. Kui midagi on puudu, antakse veateade ning vajalikud asjad tuleb �ra parandada.

<pre>$ ./configure</pre>

<b>./</b> v�imaldab k�ivitada skripti jooksvast kataloogist.

<pre>$ make</pre>

Paketis asub ka fail nimega Makefile, mis sisalfab reegleid tarkvara ehitamiseks. Kui sisestada *make* k�sk, vaadatakse just selle faili sisse.

<pre>$ sudo make install</pre>

See k�sk paigaldab paketi, �ige fail kopeeritakse arvutis �igesse kohta.

<pre>$ sudo make uninstall</pre>

*make install* k�sku kasutades tasuks olla ettevaatlik, v�ib olla �llatav kui palju tegelikult tasutal toimub. Kui hakata seda paketti hiljem eemaldama, ei pruugi k�ik oluline eemaldatud saada, kuna kasutaja ei ole tadlik t�pselt kui palju midagi s�steemi lisati. Kui n��d j�rgi m�elda, siis ehk tasuks kogu jutt *make install*i kohta �ra unustada ja kasutada hoopis k�sku  <b>*checkinstall*</b>. N�nda luuakse .deb fail, mida on kerge paigaldada ja eemaldada.

<pre>$ sudo checkinstall</pre> 

Selle k�suga sisuliselt *make install*itakse ja ehitatakse .deb pakett ning ka paigaldatakse see. See teeb hiljem eemaldamise lihtsamaks.

## Harjutus

Leida usaldusv��rselt veebilehelt l�htekoodiga programm ning paigaldada see allikast.

## K�simus

Mida peaks ALATI kasutama *make install* asemel?

## Vastus

checkinstall

