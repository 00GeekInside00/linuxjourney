# T�� kontroll

## Tunni sisu

�tleme, et t��tatakse terminali aknas ja k�ivitatud on k�sk, mille t�itmiseks kulub l�pmata palju aega. Kestaporgrammi ei saa kasutada nii kaua kui see oma �lesandega valmis saab, soov on aga t��ga j�tkata. �nneks saab t��dega kontrollida kuidas protsessid t��tavad:

<b>T�� tagaplaanile saatmine</b>

Ampersandi (&) lisamisel k�sule k�ivitub prosess tagaplaanil v�imaldades kestaprogrammi edasi kasutada. N�ide:

<pre>$ sleep 1000 &
$ sleep 1001 &
$ sleep 1002 &
</pre>

<b>Tagaplaanil olevate t��de kuvamine</b>

Tagaplaanile saadetud t�id saab vaadata.

<pre>$ jobs

[1]    Running     sleep 1000 &
[2]-   Running     sleep 1001 &
[3]+   Running     sleep 1002 &

</pre>

Kui m�ni t�� juba k�ib ja vaja on ta tagaplaanile saaata pole vaja teda peatada ja siis uuesti k�ivitada. Peata t�� ajutiselt klahvikombinatsiooniga Ctrl-Z, see j�rel sisesta <b>bg</b> k�sk, mis saadab t�� tagaplaanile.

<pre>
pete@icebox ~ $ sleep 1003
^Z
[4]+    Stopped     sleep 1003

pete@icebox ~ $ bg
[4]+    sleep 1003 &

pete@icebox ~ $ jobs

[1]    Running     sleep 1000 &
[2]    Running     sleep 1001 &
[3]-   Running     sleep 1002 &
[4]+   Running     sleep 1003 &
</pre>

<b>T�� tagaplaanilt esiplaanile toomine</b>

Et tuua t�� tagaplaanilt �ra on vaja t�psustada vaid t�� ID. Kui sisestada *fg* ilma t�psustusteta tuuakse tagasi k�ige hilisem taustat�� (t�� mille juures on +).

<pre>$ fg %1</pre>

<b>Tagaplaanil olevate t��de peatamine </b>

T��de esiplaanile liigutamise k�sule sarnases formaadis on ka nende peatamise k�sk, ikka kasutades IDd.

<pre>kill %1</pre>

## Harjutus

Liigutada t�id esi- ja tagaplaani vahel.

## K�simus

Millise k�suga n�eb tagaplaani t�id?

## Vastus

jobs

