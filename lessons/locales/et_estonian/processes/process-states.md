# Protsesside Staatused

## Tunni sisu

Vaatame uuesti *ps aux* k�sku:

<pre>$ ps aux</pre>

STAT tulbas v�ib n�ha palju v��rtusi. Linuxi protsess v�ib olla �sna paljudes erinevates olekutes.

<ul>
<li>R: *running* ehk t��tav, ootab, et protsessor temaga tegeleks</li>
<li>D: *uninterrupitble sleep* ehk siis protsess on segamatus unes, ootab, et mingi s�ndmus oma t��ga valmis saaks, n�iteks terminali sisend</li>
<li>Z: zombi, eelmises peat�kis r��giti, et zombid on t�� l�petanud protsessid, mis ootavad, et nende staatuse kohta info �ra korjataks.</li>
<li>T: peatunud, protsess on ajutiselt peatatud</li>
</ul>

## Harjutus

Tutvuda s�steemis t��tavate protsesside ja nende staatustega.

## K�simus

Millise STAT koodiga on esindatud segamatus unes protsessid?

## Vastus

D
