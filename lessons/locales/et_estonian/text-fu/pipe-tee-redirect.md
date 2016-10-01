# toru ja tee

## Tunni sisu

N��d hakkame natuke torustikuga tegelema. No mitte p�ris, aga pisut. Proovime k�sku:

<pre>$ ls -la /etc</pre>

Sa peaksid n�gema v�ga pikka nimekirja, mida on isegi natuke raske lugeda. Selle asemel, et seda faili suunata, kas ei oleks toredam, kui saaksime seda v�ljundit vaadata m�ne teise k�sga nagu less? Aga me saamegi!

<pre>$ ls -la /etc | less </pre>

Toru operaator |, mida esindab p�stkriips, lugag meil saada m�ne k�su stdout ja teha sellest teisele protsessile stdin. Meie n�ite puhul me v�tsime ls -la /etc stdout'i ja siis suunasime <i>toruga</i> less k�sule. Toru k�sk on ��rmiselt kasulik ja me j�tkame selle kasutamist aegade l�puni.

Aga kui ma tahan kirjutada oma k�su v�ljundi kahele erinevale voole? See on v�imalik j�rgmise k�suga:

<pre>$ ls | tee p�hklid.txt</pre>

SA peaksid n�gema ls v�ljundit ekraanid ja kui sa avad p�hklid.txt faili, peaksid sa n�gema seal t�pselt sama informatsiooni!
 

## Harjutus

Proovi j�rgmist k�sku:
<pre>$ ls | tee p�hklid.txt banaan.txt</pre>

## K�simus

Milline s�mbol esindab toruoperaatorit?

## Vastus

|