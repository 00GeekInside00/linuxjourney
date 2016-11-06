# yum ja apt

## Tunni sisu

Paketihalduse Batmanid! Need s�steemid sisaldavad k�ike vajaminevat, et muuta pakettide paigaldamine, eemaldamine ja muutmine lihtsaks. Sealhulgas ka s�ltuvused. Kaks k�ige popluaarsemat s�steemi on <b>yum</b> ja <b>apt</b>. Yum kuulub eksklusiivselt Red Hat perekonda ja apt Debiani omasse.

<b>Paketi paigaldamine hoidlast</b> 

<pre>
Debian: $ apt install paketi_nimi
RPM: $ yum install paketi_nimi
</pre>

<b>Paketi eemaldamine</b>

<pre>
Debian: $ apt remove paketi_nimi
RPM: $ yum erase paketi_nimi
</pre>

<b>Hoidla pakettide uuendamine</b>

Hea tava kohaselt uuendatakse paketihoidlaid, et nad oleksid ajakohased enne pakettide paigaldamist ja uuendamist.

<pre>
Debian: apt update; apt upgrade
RPM: yum update
</pre>

<b>Info saamine paigaldatud paketi kohta</b>

<pre>
Debian: apt show pekti_nimi
RPM: yum info paketi_nimi
</pre>

## Harjutus

Kasutada k�iki �pitud k�ske ja tutvuda v�ljundiga.

## K�simus

Millise k�suga kuvatakse Debianis informatsiooni paketi kohta?

## Vastus

apt show
