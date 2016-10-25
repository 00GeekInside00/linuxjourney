# /etc/shadow

## Tunni sisu

Failis /etc/shadow hoiatakse kasutajate tuvastamist puudutavat informatsiooni. Lugemiseks on vaja juurkasutaja �igusi.

<pre>$ sudo cat /etc/shadow

root:MyEPTEa$6Nonsense:15000:0:99999:7:::
</pre>

V�ib m�rgata, et sisu on /etc/passwd omale v�ga sarnane. K�ll aga on parooli koha peal hoopis kr�pteeritud salas�na. Koolonitega eraldatud v�ljad on j�rgmised:

<ol>
<li>Kr�pteeritud salas�na</li>
<li>Viimase parooli muutmise kuup�ev - v��rtus on p�evades alates 1. jaanuaris 1970. Kui selle koha peal on 0, peaks kasutaja j�rgmisel sisenemisel parooli �ra muutma</li>
<li>Minimaalne parooli vanus - p�evade arv, mida kasutaja peab ootama, enne kui v�ib salas�na muuta</li>
<li>Maximaalne parooli vanus - maksimaalne p�evade arv, kuni peab parooli muutma</li>
<li>Parooli hoiatuse periood - p�evade arv, mis on j��nud salas�na aegumiseni</li>
<li>Parooli passiivsuse periood - p�evade arv p�rast parooli aegumist kui on veel lubatud selle parooliga siseneda</li>
<li>Konto aegumise kuup�ev - kuup�ev, millal kasutaja ei saa enam sisenea</li>
<li>V�li, mis on reserveeritud mingil tulevasel eesm�rgil</li>
</ol>

Paljudes distributsioonides ei s�ltu kasutajate tuvastamine enam ainule /etc/shadow failist. Autentimist asendavad teised mehhanismid, n�iteks PAM (*Pluggable Autehntication Modules*).

## Harjutus

Vaadata /etc/shadow faili sisse.

## K�simus

K�simust pole.

## Vastus


