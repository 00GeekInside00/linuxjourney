# regex (Regulaaravaldis)

## Tunni sisu

Regulaaravaldised on v�imsad t��riistad mustril p�hineva valiku teostamiseks. See kasutab erilist kirjapilti, mis sarnaneb natuke sellele, millega oleme juba kokku puutunud, n�iteks metam�rk *.

V�tame l�bi m�ned k�ige tavalisemad regulaaravaldised, mis on pea-aegu universaalsed �ksk�ik millises programmeerimiskeeles.

Kasutame j�rgmist fraasi tests�nena:
<pre>
sally sells seashells 
by the seashore
</pre>

<b>1. Rea alustamine m�rgiga ^</b>
<pre>
<b>^by</b>
saaks vasteks rea "by the seashore"
</pre>

<b>2. Rea l�petamine m�rgiga $</b>

<pre>
seashore<b>$</b>
saaks vasteks "by the seashore"
</pre>

b>3. �he m�rgi sidumine s�mboliga .</b>

<pre>
b<b>.</b>
saaks vasteks by
</pre>

<b>4. Sulgude [] ja () kasutamine</b>

See v�ib olla natuke keerulisem, sulud lubavad meil t�psustada, mis h��likuid nende seest v�ib leida.

<pre>
d<b>[iou]</b>g
saaks vasteks: dig, dog, dug
</pre>

Kui kasutada nnne mainitud s�mbolit ^ sulgude sees, t�hendab see, et peetakse silmas k�iki t�hem�rke, peale nende mis sulgudes on.

<pre>
d<b>[^i]</b>g
saaks vasteks: dog ja dug aga mitte dig
</pre>

Sulgudes saab kasutada ka vahemikku, et suurendada soovitud t�hem�rkide hulka.

<pre>
d<b>[a-c]</b>g
leiab vasteks dag, dbg, ja dcg
</pre>

Ole hoolikas, sulud on t�stutundlikud.

<pre>
d<b>[A-C]</b>g
vasteks on dAg, dBg ja dCg kuid mitte dag, dbg ja dcg
</pre>

Ja need ongi m�ned p�hilised regulaaravaldised.

## Harjutus

Proovi kombineerida regulaaravaldisi grep'iga ja vaata l�bi m�ned failid.

<pre>
grep [siia regulaaravaldis] [fail]
</pre>

## K�simus

Millise regulaaravalidse vasteks on �ksik t�hem�rk?

## Vastus

.
