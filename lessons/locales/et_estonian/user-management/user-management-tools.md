# T��ristad kasutajate haldamiseks

## Tunni sisu

Paljud �rikeskkonnad kasuvad kasutajate, kontode ja salas�nade haldamiseks haldamise s�tsteeme. �ksikul masinal aga saab kasutajate haldamisega hakkama kui m�ne kasuliku k�skudega.

<b>Kasutajate lisamine</b>

V�ib kasutada *adduser* v�i *useadd* k�ske. *adduser* h�lmab aga rohkem kasulike omadusi, n�iteks kodukataloogi loomine. Uute kasutajate loomiseks saab muuta seadistusfaile, s�litvalt sellest, mida soovitakse m��rata vaikimisi kasutajale.

<pre>$ sudo useradd peeter</pre>

Viimane k�sk loob peetri kohta sisestuse faili /etc/passwd, loob vaikimis grupi ka lisab sisestuse ka faili /etc/shadow.

<b>Kasutajate kustutamine</b>

Kasutaja kustutamiseks v�ib kasutada *userdel* k�sku.

<pre>$ sudo userdel peeter</pre>

P�him�tteliselt annab see k�sk endast parima, et v�tta tagasi muudatused mida *useradd* failidesse tegi.

<b>Salas�na muutmine</b>

<pre>$ passwd peeter</pre>

Selle k�suga saab muuta enda v�i m�ne teise kasutaja prooli (muidugi juhul kui oled juurkasutaja).

## Harjutus

Luua uus kasutaja, muuta tema parool ja siis selle kasutajana sisse logida.

## K�simus

Millise k�suga saab muuta kasutajate paroole?

## Vastus

passwd
