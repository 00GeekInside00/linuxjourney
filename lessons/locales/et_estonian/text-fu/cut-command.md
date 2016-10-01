# cut

## Tunni sisu

�pime n��d m�ned kasulikud teksti t��tlemise k�sud. Enne kui alustame loome faili, millega hakkame tegelema. Kopeeri ja kleebi j�rgmine k�sk, kui oled seda teinud, siis lisa tabulaator laisa ja koerda vahele (hoia all Ctrl-v + TAB).

<pre>$ echo 'Kiire pruun; rebane h�ppas �le laisa  koera' > n�ide.txt</pre>

Esimesena �pime l�ikamise k�su kohta. See eraldab faili tekstist mingisuguse osa.

Et eraldada sisu t�hem�rkide nimekirja p�hjal:

<pre>$ cut -c 7 n�ide.txt</pre>

See annab v�ljundiks faili iga rea seitsmenda t�hem�rgi. Praegusel juhul on see "p". M�rka, et ka t�hikud loevad t�hem�rkidena.

Et eraldada sisu failip�hiselt, tuleb natuke muudatusi sisse viia:

<pre>$ cut -f 2 n�ide.txt</pre>

-f v�i siis v�ljalipp, l�ikab teksti p�hinedes v�ljadele. Vaikimis kasutab see eraldajana tabulaatorit, mis t�hendab, et k�ik, mida eraldab tabulaator, peeatakse omaette v�ljaks. Sa peaksid n�gema "koera" oma v�ljundina.

<pre>$ cut -f 1 -d ";" sample.txt</pre>

See muudab eraldaja tabulaatorist hoopis semikooloniks ";" ja kuna me l�ikame esimest v'lja, peaks tulemus olema hoopis "kiire pruun rebane".


## Harjutus

Mida j�rgmine k�sk teeb? Miks?

<pre>$ cut -c 5-10 n�ide.txt
$ cut -c 5- n�ide.txt
$ cut -c -5 n�ide.txt
</pre>

## K�simus

Millist k�sku sa kasutaksid, et saada iga rea esimene t�hem�rk?

## Vastus

cut -c 1
