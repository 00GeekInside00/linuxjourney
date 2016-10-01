# stdin (Standard In)

## Tunni sisu

Eelmises tunnis �ppisime, et me saame kasutada erinevaid stdout voogusid, n�iteks faili v�i ekraani. Samamoodi on olemas ka standardsisendi (stdin) voogusid. Teame, et onolemas stdin seadmetelt nagu klaviatuur, kuid me v�ime kasutada ka faile, teiste protsesside v�ljundeid ning ka terminali. Vaatame n�idet.

Kasutame selle n�ite jaoks eelmise tunni p�hklid.txt faili. Meenuta, et seal oli sees tekst Hello World.

<pre>$ cat <b>&lt;</b> p�hklid.txt <b>&gt;</b> banaan.txt </pre> 

Just nagu meil oli <b>&gt;</b> stdout �mbersuunamiseks, on meil <b>&lt;</b> stdin �mbersuunamise jaoks.

Tavaliselt saadaksid sa cat k�su puhul sellele faili ja sellest saab stdin, praegusel juhul aga suunasime me stdin'ks p�hklid.txt. Sedasi suunatakse cat p�hklid.txt v�ljund �mber faili mimega banaan.txt

## Harjutus

Proovi paari k�sku:
<pre>
$ echo <b>&lt;</b> p�hklid.txt <b>&gt;</b> banaan.txt
$ ls <b>&lt;</b> p�hklid.txt <b>&gt;</b> banaan.txt
$ pwd <b>&lt;</b> p�hklid.txt <b>&gt;</b> banaan.txt
</pre>

## K�simus

Millise k�suga suunad sa �mber stdin?

## Vastus

<
