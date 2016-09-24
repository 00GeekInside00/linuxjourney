# rm (Remove)

## Tunni sisu

N��d kui mulle tundub, et meil vist on liiga palju faile, eemaldaks m�ned. Selleks, et faile eemaldada, kasutame rm k�sku. Rm (inglise keeles remove ehk eemalda) k�sku kasutatakse, et kustutada faile ja katalooge.

<pre>$ rm fail1</pre>

Ole rm kasutamisega ettevaatlik, sul ei ole maagilist pr�gikasti, kust hiljem eemaldatud faile v�lja �ngitseda. Kui nad l�inud, siis nad igaveseks l�inud, seega ole t�helepanelik.

�nneks on �les seatud turvameetmed, et p�ris iga�ks ei saaks eemaldada olulisi faile. Kirjutamise vastu kaitstud failid k�sivad sult kinnitust enne kui sa nad �ra kustutad. Samuti ei ole kirjutamise vastu kaitstud kataloogi niisama lihtne eemaldada.

Kui sind k�ik see eelneb ei huvita, siis saad sa igal juhul eemaldada mingid failid.

<pre>$ rm -f fail1</pre>

-f (inflise keeles force ehk j�uga) valik �tleb rm k�sule, et see eemaldaks k�ik failid hoolimata sellest, kas nad on kirjutamise vastu kaitstud v�i mitte. Seda ilma, et sult enne �le k�sitakse (kui sul on selleks vastavad volitused).

<pre>$ rm -i fail</pre>

Sanraselt teistele k�skudele, annab lipu -i lisamine sulle enne faili v�i kataloogi kustutamist v�imaluse valida, kas sa ikka soovid seda teha.

<pre>$ rm -r kataloog</pre>

Kataloogi ei saa niisama lihtsalt eemaldada, sul on vaja lisada lipp -r (rekursiivne), et eemaldatakse k�ik failid ja alamkataloogid, mis seal v�ivad olla.

Kataloogi saab eemaldada rmdir k�suga.

<pre>$ rmdir kataloog</pre>

## Harjutus

<ol>
<li>Loo fail nimega -fail (�ra unusta sidekriipsu!).</li>
<li>Eemalda see fail.</li>
</ol>

## K�simus

Kuidas eemaldada fail nimega minufail?

## Vastus

rm minufail