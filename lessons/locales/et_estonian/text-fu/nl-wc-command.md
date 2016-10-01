# wc ja nl

## Tunni sisu

wc (inglise keele word count ehk s�nade loendus) k�sk kuvab faili t�ieliku s�nade hulga.

<pre>$ wc /etc/passwd
 96     265    5925 /etc/passwd
</pre>

Vastavalt v�ljundile on kuvatud ridade, s�nade ja vaitide arv.

Selleks, et ainult �hte v�lja kuvataks, kasuta vastavalt -l, -w v�i -c.

<pre>$ wc -l /etc/passwd
96</pre>

Veel �ks k�sk, millega saab faili ridade arvu teada, on nl (number lines ehk ridade number).

<pre>
fail1.txt
mulle
meeldivad
kilpkonnad
</pre>

<pre>$ nl file1.txt
1. mulle
2. meeldivad
3. kilpkonnad
</pre>

## Harjutus

Kuidas sa saaksid nl k�sku kasutades faili l�pliku ridade arvu ilma, et peaksid kogu v�ljundil l�bi vaatama? Vihje: Kasuta m�ningaid teisi k�ske, mida sellel kursusel juba �ppinud oled.

## K�simus

Millist k�sku kasutaksid, et saada failist ainult l�plik s�nade arv.

## Vastus

wc -w
