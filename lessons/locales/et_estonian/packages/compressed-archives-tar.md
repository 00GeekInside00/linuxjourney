# tar ja gzip

## Tunni sisu

Enne kui r��ida pakettide paigaldamisest ja erinevatest haldusprogrammidest, v�iks r��kida failide arhiveerimisest ja tihendamisest, sest neid tuleb kindlasti internetist tarkvara jahtides ette.

Failid, mille laiend on .rar ja .zip on arhiivifailid. Nende sees on veel omakorda palju faile, kuid nad on kenasti �heks arhiivina tuntud failiks kokku pakitud.

<b>Failide tihendamine ja *gzip*<b/>

*Gzip* on programm, mida kasutatakse failide tihendamiseks Linuxis, nende laiendiks on .gz.

Faili tihendamiseks:
<pre>$ gzip minulahefail</pre>

Lahti pakkimiseks:
<pre>$ gunzip minulahefail.gz</pre>

<b>Arhiivide loomine ja tar</b>
Kahjuks ei saa *gzip* lisada arhiivi mitut faili. �nneks aga saab seda teha *tar*ga. Kui luua sellega arhiiv, on faililaiendiks .tar.

<pre>$ tar cvf minutarfail.tar minulahefail1 minulahefail 2</pre>


<ul>
<li>c - loomine</li>
<li>v - �tleme programmile, et see kannaks ette, mida ta teeb</li>
<li>f - selle v�tme j�rel peab tulema *tar* faili nimi, kui luua uus fail tuleb nimi v�lja m�elda/li>
</ul>

<b>Arhiivide lahti pakkimine ja *tar*</b>

Et pakkida lahti *tar* faili:

<pre>$ tar xvf minutarfail.tar</pre>

<ul>
<li>x - lahtipakkimine</li>
<li>v - �tleme programmile, et see kannaks ette, mida ta teeb</li>
<li>f - fail, mida soovitakse lahti pakkida</li>
</ul>

<b>Arhiivide tihendamine ja lahti pakkimine *gzip* ja *tar*iga</b>

Tihti v�ib leida *tar* faile, mis on tihendatud: minutihendatudarhiiv.tar.gz. Sellisel juhul tuleb hakkata tegutsema v�ljast poolt sissepoole: esiteks eemaldame tihenduse *gunzip*iga ja seej�rel pakime *tar* faili lahti. On ka v�imalik kasutada <b>z</b> varianti, mis �tleb *tar*ile, et on vaja kasutada *gzip* v�i *gunzip* utiliiti.

Tihendatud *tar* faili loomine:
<pre>$ tar czf minufail.tar.gz</pre>

Tihenduse eemaldamine ja lahti pakkimine:
<pre>$ tar xzf fail.tar</pre>

Inglise keele tundmine aitab k�sku meeles pidada: e<b>X</b>tract all <b>Z</b>ee <b>F</b>iles!

*tar* on �ks nendest k�skudest, mis on v�ga oluline kuid, mida kunagi ei suudeta p�riselt meelde j�tta: <a href="https://xkcd.com/1168/">https://xkcd.com/1168/</a>

<b>Teised utiliidid</b>

Mida rohkem kasutada Linuxit, seda rohkem puutub kokku erinevate arhiveerimis- ja tihendust��pidega, n�itkes *bzip2*, *compress*, *zip*, *unzip* jne, kuid need on natuke v�hem levinud. Tasub meelde j�tta, et erinevad utuliidid kasutavad erinevaid k�ske.

## Harjutus

Tutvuda *tar*i dokumentatsiooniga ja uurida *man*lehek�ljelt erinevate kasutusv�imaluste kohta.

## K�simus

Millise v�tmega luuakse arhiive?

## Vastus

c
