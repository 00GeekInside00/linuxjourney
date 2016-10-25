# ps (Protsessid)

## Tunni sisu

Protsessid on arvutis t��tavad programmid. Neid haldab tuum ja neil k�igil on oma ID, mida nimetatakse <b>protsessi IDks (PID)</b>. Need IDd jagatakse v�lja protsessside loomise j�rjekorras.

*ps* k�sku sisestades saab n�ha nimekirja t��tavatest protsessidest:

<pre>$ ps

PID        TTY     STAT   TIME          CMD
41230    pts/4    Ss        00:00:00     bash
51224    pts/4    R+        00:00:00     ps
</pre>

Kiire �lesv�te protsesside kohta annab j�rgmist infot:

<ul>
<li>PID: Protsessi ID</li>
<li>TTY: Protsessiga seotud terminal (sellest pikemalt veidi hiljem)</li>
<li>STAT: Protsessi staatuse kood</li>
<li>TIME: Kumulatiivne protsessori kasutamise aeg</li>
<li>CMD: K�su/k�ivitatud rakenduse nimi</li>
</ul>

*Ps*i *man* lehet v�ib leida palju erinevaid v�imalusi selle k�su sisestamiseks. Need erinevad veidi s�ltuvalt, millist variant soovitatakse kasutada - BSG, GNU v�i Unix. T�en�olisel ton BSD stiil teistest natuke populaarsem, seega kasutatakse sellel kursusel seda. Uudishimu rahuldamiseks v�ib �elda, et erunevus seisneb selles mitut kriipsu kasutatakse ja lippudes.
 
<pre>$ ps aux</pre>

<b>a</b> kuvab k�ik t��tavad protsessid, kaasaaravtud need, mis t��tavad teiste kasutajate all. <b>u</b> kuvab protsesside kohta rohkem detaile ja viimaks, <b>x</b> kuvab k�ik protsessid, millega ei ole TTYd seostatud. Nened protsessidel on ? TTY v�ljas. Selline asi on v�ga levinud deemoni protsessides, mis seotud s�steemi k�ivitumisega.

Selle k�suga on n�ga oluliselt rohkem v�lju. Neid pole vaja k�iki meelde j�tta, j�rgmises peat�kkis, kus r��gitakseprotsessidest l�hemalt, r��gitakse neist uuesti:

<ul>
<li>USER: Kehtiv kasutaja (see kelle ligip��su�igusi kasutatakse)</li>
<li>PID: Protsessi ID</li>
<li>%CPU: Protessori aja kasutuse suhe aega, mis protsess on t��tanud</li>
<li>%MEM: Ratio of the process's resident set size to the physical memory on the machine</li>
<li>VSZ: Protsessi virtuaalm�lu kasutus</li>
<li>RSS: Resident set size, saalimata f��siline m�lu, mida tegum on kasutanud</li>
<li>TTY: Protessiga seostatud terminal</li>
<li>STAT: Protsessi staatuse kood</li>
<li>START: Protsessi k�ivitumise aeg</li>
<li>TIME: Kumulatiivne protsessori kasutamise aeg</li>
<li>COMMAND: K�su/k�ivitatud rakenduse nimi</li>
</ul> 

*ps* k�su vaatamine v�ib muutuda t�likaks, hetkel uurime k�ige rohkem v�lju PID, STAT ja COMMAND.

Teine v�ga kasulik k�sk on *top*. See kuvab sulle t��tavate protsesside kohta juba mitte enam hetke �lesv�tet, vaid jooksvat informatsiooni. Vaikimisi uuendatakse kuva iga 10 sekundi j�rel. *Top* on ��rmisel kasulik vahend kui on vajalik teada, milised protsessid kasutavad suurem m��ral arbuti ressursse.

<pre>$ top</pre>

## Harjutus

Kasutada *top*o erinevate lippudega ja p��rata t�helepanu sellele, kuidas muutub kuvatav info.

## K�simus

Millise lipuga kuvatakse protsesside kohta detailset infot?

## Vastus

u
