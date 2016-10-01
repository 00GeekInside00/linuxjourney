# sort

## Tunni sisu

Sort k�sk on kasulik ridade sorteerimiseks.

<pre>
fail1.txt
koer
lehm
kass
elevant
lind

$ sort fail1.txt
elevenat
kass
koer
lehm
lind
</pre>

Saab teha ka tagurpidise sorteerimise:

<pre>$ sort -r fail1.txt
lind
lehm
koer
kass
elevant
</pre>

Samuti ka numbrilise v��rtuse p�hjal:

<pre>$ sort -n fail1.txt
--pean j�rgi proovima--
</pre>

## Harjutus

Sort k�su t�eline j�ud tuleneb v�imalusest kasutada seda koos teiste k�skudega. Proovi j�rgmist k�sku ja vaata, mis juhtub?

<pre>$ ls /etc | sort -rn</pre>

## K�simus

Millise k�suga saab teha tagurpidi soreteerimist?

## Vastus

-r
