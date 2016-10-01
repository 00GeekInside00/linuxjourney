# head

## Tunni sisu

�tleme, et meil on v�ga pikk fail, meil on isegi mitu, mille hulgast valida, proovi cat /var/log/syslog. Sa peaksid n�gema lehek�lgede kaupa teksti.  Mis siis kui ma tahaksid n�ha ainult paari eimest teksti faili rida? Seda saame teha k�suga head. Vaikimisi n�itab head k�sk sulle faili esimest 10 rida.

<pre>$ head /var/log/syslog</pre>

Sa saad ka muuta ridade arvu selliseks, mis sulle rohkem meeldib. �tleme, et tahad n�ha hoopis esimest 15 rida.

<pre>$ head -n 15 /var/log/syslog</pre>

Lipp -n esineb ridade arvu.

## Harjutus

Mida teeb j�rgnev k�sk ja miks?

<pre>$ head -c 15 /var/log/syslog</pre>

## K�simus

Millist lippu kasutad, kui tahad muuta head k�suga vaadeldavate ridade arvu?

## Vastus

-n

