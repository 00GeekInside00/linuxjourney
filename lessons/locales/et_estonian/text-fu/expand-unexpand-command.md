# expand ja unexpand

## Tunni sisu

Cut k�su peat�kis oli meil n�ide.txt fail, milles oli kasutatud tabulaatorit. Tavaliselt peaks see olema m�rgatavalt n�ha, kuid m�ned tekstifailid ei n�ita seda piisavalt h�sti. Tabulaator ei pruugi olla parim eraldaja, mida tekstifailis kasutada.
Et muuta k�ik oma tabulaatorid t�hikuteks, kasuta expand k�sku.

<pre>$ expand n�ide.txt</pre>

See k�sk tr�kib v�ljundi, kus k�ik tabulaatorid on muudetud grupiks t�hikuteks. Et see v�ljund faili salvestada, kasuta v�ljundi �mbersuunamist, nagu all n�idatud.

<pre>$ expand n�ide.txt > tulemus.txt</pre>

Vastandile expand k�sule, saame muuta ka grupi t�hikuid tabulaatoriks. Kasutame selleks k�sku unexpand:

<pre>$ unexpand -a tulemus.txt</pre>

## Harjutus

Mis juhtun kui sisestad lihtsalt expand ilma faili sisendita?

## K�simus

Millise k�suga muudetakse tabulaatorid t�hikuteks?

## Vastus

expand
