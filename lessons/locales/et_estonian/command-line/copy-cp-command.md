# cp (Copy)

## Tunni sisu

Teeme m�nest failist koopiad. Sarnaselt teistes operatsioonis�steemis kopeerimisele ja kleepimisele v�imaldab shell meil seda isegi veel lihtsamalt teha.

<pre>$ cp minuvingefail /home/pete/Dokumendid/vingeddokud</pre>

minuvingefail on see fail, mida sa tahad kopeerida ja /home/pete/Dokumendid/vingeddokud on see, kuhu sa tahad seda kopeerida.

Sa saad kopeerida ka korraga mitmeid faile ja katalooge, ning kasutada metam�rki. Metam�rk on selline t�hem�rk, mis v�ib asendada mingil mustril p�hinevat valikut, andes sulle otsimiseks rohkem vabadust. Sa v�id pandlikkuse m�ttes kasutada metam�rke iga k�su juures.


<ul>
<li>* metam�rkide metam�rk, kasutatakse, et esinada �ksk�ik millist t�hem�rki v�i s�net.</li>
<li>? esindab �hte t�hem�ri</li>
<li>[] asindab �ksk�ik millist kantsulgudesse kirjutatud t�hem�rki</li>
</ul>

<pre>$ cp *.jpg /home/pete/Pildid</pre>

See k�sk kopeerib k�ik .jpg laiendiga failid sinu jooksvast kataloogist kataloogi Pildid.

P�ris kasulik on kasutada ka -r lippu, see kopeerib tagasiulatuvalt kataloogis asuvad kataloogid ja failid.

Proovi kasutada cp k�sku, et kopeerida Dokumentide kausta m�ni kataloog, milles on m�ned failid sees. See ei t��tanud, eks? Seda selle p�rast, et sa pead kopeerima ka k�ik failid ja kataloogid, mis seal kaustas on k�suga -r.

<pre>$ cp -r K�rvits/ /home/pete/Dokumendid</pre>

Oluline on panna t�hele, et kui sa kopeerid faili kataloogi, milles on sama nimega fail, siis see fail kirjutatakse �le kopeeritava failiga. See ei ole v�ga bueno, kui sul on seal m�ni fail, mida sa ei taha kogemata �lekirjutada. Sa v�id kasutada lippu -i (interaktiivne), et sult k�sitaks enne kui fail �lekirjutatakse.

<pre>$ cp -i minuvingefail /home/pete/Pildid</pre>

## Harjutus

Kopeeri m�nda faili, kuid ole ettevaatlik, et sa midagi olulist �le ei kirjutaks.

## K�simus

Millist lippu on sul t�psustamiseks vaja, kui soovid kopeeria kataloogi?

## Vastus

-r