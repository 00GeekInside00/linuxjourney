# alias

## Tunni sisu

M�nikord v�ib muutuda k�skude sisestamine v�ga korduvaks, v�ik on sul on vaja kirjutada v�ga pikka k�sku mitu korda. Sellisel juhul oleks parem kasutada selleks aliast. K�sule aliase loomiseks, pead lihtsalt t�psustama aliase nime ja seostama selle k�suga.

<pre>$ alias foobar='ls -la'</pre>

N��d v�id ls -ls asemel kirjutada foobar, ja see k�ivitab k�su. P�ris viisakas v�rk. Pea meelest, et aliased ei s�ili, kui pead arvuti taask�vitama. Selleks peab looma permanentse aliase:

<pre>~/.bashrc</pre>

v�i m�nda teise sarnasesse faili, kui soovid, et see s�iliks ka p�rst taask�ivitamist.

Aliase saab eemaldada unalias k�suga:

<pre>$ unalias foobar</pre>

## Harjutus

Loo m�ned aliased ja eemalda nad.

## K�simus

Millise k�suga luuakse alias?

## Vastus

alias
