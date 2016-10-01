# stdout (Standard Out)

## Tunni sisu

Praguseks oleme juba p�ris paljude k�skude ja nende v�ljunditega tuttavaks saanud ja see viib meid ka edasi j�rgmise teemani: sisend/v�ljund vood. Sisestame j�rgmise k�su ja p�rast arutame, kuidas see t��tab:

<pre>$ echo Hello World > p�hklid.txt</pre>

Mis just praegu juhtus? Aga mine kontrolli seda kataloogi, kus sa selle k�su k�ivitasid ja pane end valmis, sest sa peaksid sealt leidma faili nimega p�hklid.txt. Kui sa sinna sisse vaatad, siis peaksid leidma teksti Hello World. Selle �he k�suga juhtus p�ris palju, vaatame seda jupp haaval.

Vaatame esimest osa:

<pre>$ echo Hello World</pre>

Me teame, et see tr�kib ekraanile Hello World, aga kuidas? Protsessid kasutavad sisend-v�ljund voogusid, et v�tta vastu sisendandmeid ja v�ljastada v�ljundeid. Vaikimisi v�tab echo k�sk sisendi (standard sisend v�i stdin) klaviatuurilt ja tagastab v�ljundi (standard v�ljund v�i stdout) ekraanile. Seep�rast, kuvatakse su ekraanile Hello World, kui sa sisestad shelli echo Hello World. Sisend-v�ljundi �mbersuunamisega saame aga seda vaikimisi k�itumist muuta, see annab meile failide osas suurema paindlikuse.

Vaatame, mis selle k�suga edasi juhtus:

<pre> > </pre>

> on �mbersuunamise operaator, mis laseb meil muuta seda, kuhu suunatakse standardv�ljund. See lubab meil suunata echo Hello Worldi v�ljundi ekraani asemel faili. Kui sellist faili veel olemas ei ole, siis see luuakse. Kui see aga on olemas, siis kirjutatakse see �le (olenevalt shellist, saad sa lisada k�sule lipu, et sellist olukorda v�ltida).

Ja nii p�him�tteliselt stdout �mbersuunamine t��tabki!

�tleme aga, et ma ei taha oma p�hklid.txt faili �lekirjutada. �nneks on selle jaoks ja olemas �mbersuunamise operaator, >>:


<pre>$ echo Hello World >> p�hklid.txt</pre>

See lisab Hello Worldi p�hklid.txt faili l�ppu. Kui aga faili eelnevalt ei eksisteerinud, siis luuakse see, justnagu > �mbersuunamisegagi.


## Harjutus

Proovi paari k�sku:

<pre>
$ ls -l /var/log > minuv�ljund.txt
$ echo Hello World > rm
$ > mingifail.txt 
</pre>

## K�simus

Millist k�sku kasutad kui tahad v�ljundi lisada olemasoleva faili l�ppu?

## Vastus

>>
