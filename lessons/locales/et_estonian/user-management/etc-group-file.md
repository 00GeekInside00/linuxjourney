# /etc/group

## Tunni sisu

Kasutajate haldamiseks kasutatakse veel �hte faili. /etc/group v�imaldab erinevate �igustega gruppe.

<pre>$ cat /etc/group

root:*:0:pete
</pre>

Sarnaselt /etc/shadow failile, on /etc/group v�ljad j�rgmised:

<ol>
<li>Grupi nimi</li>
<li>Grupi salas�na - tegelikult pole vajadust seada grupile paroli,pigem on tavap�rane t�stetud �iguste kasutamine, nagu n�iteks *sudo* puhul. Vaikimis v��rtus on "*".</li>
<li>Grupi ID (GID)</li>
<li>Nimekiri kasutajatest - kastuajate gruppi kuuluvust saab k�sitsi m��rata</li>
</ol> 

## Harjutus

K�ivitada k�sk <b>*groups*</b>. Mida kuvatakse?

## K�simus

Mis on juurkasutaja GID?

## Vastus

0
