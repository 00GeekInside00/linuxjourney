# mv (Move)

## Tunni sisu

Kasutatakse failide liigutamiseks, aga ka �mbernimetamisek. Lippude ja toimimise poolest on see cp k�sule �sna sarnane.

Faile saab �mbernimetada nii:

<pre>$ mv vanafail uusfail</pre>

V�i sa v�id liigutada faili hoopis teise kataloogi:

<pre>$ mv fail2 /home/pete/Dokumendid</pre>

Ja liigutada rohkem kui �hte faili:

<pre>$ mv fail_1 fail_2 /mingikataloog</pre>

Katalooge saab ka �mbernimetada:

<pre>$ mv kataloog1 kataloog2</pre>

Nagu ka cp, kui sa liigutad faili v�i kataloogi, siis see kirjutab �le, kui seal kataloogis juba midagi samanimelist on. Seega, kasuta -i lippu, et saaksid teate enne kui midagi �le kirjutatakse.

<pre>$ mv -i kataloog1 kataloog2</pre>

Aga �tleme, et sa tahad liigutada faili n�nda, et see kirjutaks eelmise �le. Sa v�id teha failist varuvariandi, sel juhul nimetatakse vana fail �mber ~ s�mboliga.

<pre>$ mv -b kataloog1 kataloog2</pre>

## Harjutus

Anna m�nele failile uus nimi, seej�rel liiguta see teise kataloogi.

## K�simus

Kuidas sa annad failile nimega kass uue nime koer?

## Vastus

mv cat dog