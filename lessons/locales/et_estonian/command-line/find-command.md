# find

## Tunni sisu

Meil on s�steemis palju faile ning nendest �he konkreetse leidmine v�ib muutuda veidi keeruliseks. Saame selle jaoks kasutada k�sku find!

<pre>$ find /home -name kutsikad.jpg</pre>

Kui kasutad find k�sku, pead t�psustama, millisest kataloogist tuleb faili otsida, mida sa otsid. Praegusel juhul otsime faili nime (name) kutsikad.jpg j�rgi.

Sa v�id ka t�psustada, millist t��pi faili sa leida p��ad.

<pre>$ find /home -type d -name MinuKaust</pre>

Nagu m�rkasid, siis ma panin faili t��pbiks d kataloogi jaoks ning samal ajal ma otsin endiselt nime j�rgi MinuKaust.

Lahe asi, mida silmas pidada, on see, et find ei piirdu otsimisega t�psustatud kataloogist, see otsib ka k�ikv�imalikes alamkataloogidest.

## Harjutus

<ol>
<li>Leia juurkataloogist fail, mille nimes on s�na net.</li>
</ol>

## K�simus

Kuidas pean find k�sku t�psustama, kui tahan otsida nime j�rgi?

## Vastus

-name