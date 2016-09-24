# pwd (Print Working Directory)

## Tunni sisu

Linuxis on k�ik asjad failid. Mida s�gavamale Linuxi maailma sa r�ndad, seda paremini hakkad sa seda m�istma. Hetkel pea see aga lihtsalt meeles. K�ik failid on organiseeritud hierarhilise kataloogipuuna. Failis�steemi esimese kataloogi nimi on v�ga asjakohaselt juurkataloog. Juur kataloogis asub palju kaustu ja faile, milles omakorda asub veel kaustu ja faile jne. N�ide, kuidas kataloogi puu v�ib v�lja n�ha:

<pre>/
|-- bin
|   |-- file1
|   |-- file2
|-- etc
|   |-- file3
|   `-- directory1
|       |-- file4
|       `-- file5
|-- home
|-- var
</pre>

Failide ja Kataloogide puhul r��gitakse nende asukohast. Kui sul oleks kaust nimega home, mille sees oleks pete nimeline kaust, mille sees omakorda oleks kaust Filmid, siis n�eks selle asukoht v�lja j�rgmine: /home/pete/Filmid. Lihtne, v�i mis?

Failis�steemis, nagu ka reaalses maailmas, teeb navigeerumise oluliselt lihtsamaks, kui sa tead, kus sa asud ja kuhu sa minna tahad. Selleks, et n�ha, kus sa asud, v�id kasutada k�sku pwd. T�lkes t�hendab see k�sk "kuva jooksev kataloog" ning see lihtsalt n�itabki sulle, millises kataloogis sa asud. Pane t�hele, et asukoht algab juurkataloogist.


<pre>$ pwd</pre>

Kus sa oled? Kus mina olen? Proovi j�rgi.

## Harjutus

Selles peat�kis harjust ei ole.

## K�simus

Kuidas sa saad teada, millises kataloogis sa parasjagu oled?

##

pwd