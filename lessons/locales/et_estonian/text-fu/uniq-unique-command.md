# uniq (Unique)

## Tunni sisu

Uniq (unikaalne) k�sk on veel �ks kasulik t��rist teksti t��tlemiseks.

�tleme, et sul on �hest failist mitu koopiat:


<pre>
lugemine.txt
raamat
raamat
ajaleht
ajaleht
artikkel
artikkel
ajakiri
</pre>

ja sa tahad korduvatest eksemplaridest lahti saada. Selleks saab kasutada uniq k�sku:

<pre>$ uniq lugemin.txt
raamat
ajaleht
artikkel
ajakiri</pre>

Kuvame iga rea kohta nende esinemissageduse:

<pre>$ uniq -c lugemine.txt
2 raamat
2 ajaleht
2 artikkel
1 ajakiri</pre>

V�tame ainult unikaalsed v��rtused:

<pre>$ uniq -u lugemine.txt
ajakiri</pre>

V�tame ainult korduvad v��rtused:

<pre>$ uniq -d lugemine.txt
raamat
ajaleht
artikkel
</pre>

<b>M�rkus</b> : uniq ei tuvasta korduvaid ridu juhul, kui nad ei asu k�rvuti. N�iteks:

�tleme, et sul on fail, mille korduvad read ei asu k�rvuti:

<pre>
lugemine.txt
raamat
ajaleht
raamat
ajaleht
artikkel
ajakiri
artikkel
</pre>

<pre>$ uniq lugemine.tx
raamat
ajaleht
raamat
ajaleht
artikkel
ajakiri
artikkelt</pre>

Uniq'i tagastatud v�ljund sisaldab k�iki kirjed, erinevalt esimesest n�itest.

Et sellest piirangust vabaneda, v�ime kasutada uniq k�sku koos sort k�suga:

<pre>
$ sort lugemine.txt | uinq
artikkel
raamat
ajakiri
ajaleht</pre>

## Harjutus

Milline oleks v�ljud kui prooviksid sisestada uniq -uc?

## K�simus

Millist k�sku kasutaksid, et vabaneda failis kordustest?

## Vastus

uniq
