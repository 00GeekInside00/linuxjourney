# cd (Change Directory)

## Tunni sisu

N��d, kui sa tead, kus sa oled, vaatame, kas meil �nnestub failis�steemis pisut ringi liikuda. Pea meeles, et liikumiseks peame kasutama asukoti. Asukoha m��ramiseks on kaks v�imalust: absoluutne ja suhteline.

<ul>
<li>Absoluutne asukoht: See on faili asukoht alates juurkataloogist. Juur on meil see k�ige olulisem tegelane. Juurkataloogi kuvatakse tavaliselt kaldkriipsuga. Kui asukoha alguses on /, siis t�hendab, et sa alustad juurkataloogist. N�iteks /home/pete/T��laud.</li>

<li>Suhteline asukoht: See on faili asukoht alates sinu praegusest asukohast failis�steemis. Kui ma asuksin praegu /home/pete/Dokumendid ja tahaksin liikuda Dokumentides asuvasse Arced kataloogi, siis ei ole mul vaja t�psustada kogu asukohta alates juurest, ma v�in lihtsalt minna arved/ .</li>
</ul>

N��d, kui me teame kuidas asukohad toimivad, on meil vaja midagi, mis aitaks meil liikuda soovitud kataloogi. �nneks on meil cd v�i siis "muuda kataloogi", et seda saavutada.

<pre>$ cd /home/pete/Pildid</pre>

N��d ma muutsin oma asukohaks home/pete/Pildid.

Selles kasutas on mul aga katalaoog Hawaii, ma saan sinna liikuda n�nda:

<pre>$ cd Hawaii</pre>

M�rkasid, et ma kasutasin ainult kausta nime? Sain nii teha, kuna mu asukoht juba oli /home/pete/Pildid

V�ib muutuda p�ris v�sitavaks, kui kogu aeg peab kasutama absoluutseid v�i suhtelisi asukohti. �nneks on meie abistamiseks olemas otseteed.

<ul>
<li>. (praegune kataloog). See on kataloog, milles sa asud. </li>
<li>.. (eelnev kataloog). Viib su praeguse kataloogi �lemkataloogi.</li>
<li>~ (home kataloog). See on vaikimisi su kodukataloog, n�iteks /home/pete.</li>
<li>- (eelmine kataloog). Viib su kataloogi, kus sa viimati asusid.</li>
</ul>

<pre>$ cd .
$ cd ..
$ cd ~
$ cd -
</pre>
Proovi need �ra!

<ol>
<li>Kuhu sa satud, kui sisestad cd k�su ilma t�iendava infota?</li>
</ol>

## K�simus

Kui su asukoht on /home/pete/Pildid ja sa tahad minna kataloogi /home/pete, siis millist otseteed oleks hea kasutada?

## Vastus

cd ..