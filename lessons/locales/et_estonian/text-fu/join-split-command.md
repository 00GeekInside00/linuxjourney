# Join ja split

## Tunni sisu

Join k�sk lubab sul �hise v�lja kaudu liita kokku mitu faili:

�tleme, et mul on kaks faili, mida ma tahan kokku liita:

<pre>fail1.txt
1 John
2 Jane
3 Mary

fail2.txt
1 Doe
2 Doe
3 Sue

$ join fail1.txt fail2.txt
1 John Doe
2 Jane Doe
3 Mary Sue
</pre>

N�gid kuidas see mu failid kokku liitis? Nad �hendatakse vaikimisi esimese v�lja kaudu, mis peavad olema identsed. Kui nad seda ei ole, saad sa neid sorteerida, nii et praegusel juhul �hendatakse neid 1, 2 ,3 abil.

Kuidas sa liidaksid j�rgmisi faile?

<pre>fail1.txt
John 1
Jane 2
Mary 3

fail2.txt
1 Doe
2 Doe
3 Sue
</pre>

Et seda faili �hendada, pead sa t�psustama milliseid v�lju �hendada. Hetkel me tahame v�lja 2 fail1.txt'st ja v�lja 2 fail2.txt's, seega n�eb k�sk v�lja nii:

<pre>
$ join -1 2 -2 1 fail1.txt fail2.txt
1 John Doe
2 Jane Doe
3 Mary Sue
</pre>

-1 viitab fail1.txt'le ja -2 viitab fail2.txt'le. P�ris uhke. �hte faili on aga v�imalik ka jagada mitme faili vahel kui kasutad split k�sku:

<pre>$ split mingifail</pre>

Nii jagadakse fail mitmeks failiks, vaikimisi eraldatakse nad, kui 1000 rea limiit t�is saab. Failid nimetatakse vaikimisi x**.

## Harjutus

Liida kokku kaks faili, milles on erinev arv ridu. Mis juhtub?

## K�simus

Millise k�suga liidaksid sa kokku failid kass, koer ja lehm?

## Vastus

join kass koer lehm
