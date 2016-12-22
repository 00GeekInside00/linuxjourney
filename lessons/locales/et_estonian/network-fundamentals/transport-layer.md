# Transpordikiht

## Tunni sisu

Transpordikiht v�imaldab edastada andmeid v�rgule loetavas keeles. See jagab kasutaja andmed t�kkideks, mida seej�rel edastatakse ja pannakse hiljem j�lle �iges j�rjekorras kokku. Neid t�kke nimetatakse segmentideks. Segmendid teevad andete edastamise lihtsamaks.

<b>Pordid</b>

Kuigi me teame IP aadressi j�rgi kuhu me saadame admed, ei piisa sellest, et saata andmed kindlale protsessile v�i teenusele. Teenused nagu HTTP kasutavad kommunikatsioonikanaleid portide n�ol. Kui tahame saata andmeid veebilehele, saadame me andmed �le HTTP pordi (port 80). Lisaks segmentide moodustamisele, lisab transpordikiht sellele ka l�hte- ja sihtkoha pordi. T�nu sellele teab vastuv�ttev pool, millist porti kasutada.

<b>UDP</b>

Kaks populaarset transpordiprotokolli on UDP ja TCP. Tutvustame UDP'd ainult kergelt ja veedame suurema aja TCP'ga, kuna seda kasutatakse t��pilisemalt.

UDP ei ole usaldusv��rne meetod andmete edastamiseks, tegelikult seda isegi ei huvita, kas kasutaja saab k�ik andmed k�tte v�i mitte. See v�ib k�lada halvasti, kuid ka UDP'l on oma koht, n�iteks meedia voogesituses. Ei ole ju hullu kui m�ned raamid ei j�ua kohale, kuid selle eest edastatakse andmeid kiiremini.

<b>TCP</b>

TCP pakub usaldusv��rset �hendusele orienteeritud andete edastamist. TCP kasutab porte saatmaks andmeid hostide vahel. Rakendus avab �henduse m�lema hosti juures. Et luua �hendus, kasutatakse TCP k�epigistust.

<ul>
<li>Klient saadab serverile �henduse palvega SYN segmendi.</li>
<li>Server saadab kliendile SYN-ACK segmendi, et kinnitada kliendi �henduse palvet</li>
<li>Klient saadab serverile ACK segmendi, et kinnitada serveri �henduse palvet</li>
</ul>

Kui see �hendus on saavutatud, v�ib �le selle admeid vahetada. Andmeid saadetakse segmentidena ja neil on j�rjekorra numbrid, et nad p�rast kohale toimetamist j�lle �igesti kokku panna. Meie e-kirja n�ites, kinnitab traspordikiht pordi (25) sihtpunkti sihtpordina.

## Harjutus

Harjutust pole.

## K�simus

Milline on usaldusv��rne transpordiprotokoll?

## Vastus

TCP
