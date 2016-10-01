# grep

## Tunni sisu

Grep on v�ga t�en�oliselt k�ige tavalisem teksti t��tlemise k�sk, mida sa kasutama hakkad. See lubab sul otsida failist t�em�rke, mis vastavad teatud mustrile. Mis siis kui sa tahad teada, kas mingi fail eksisteerib mingis konkreetses kataloogis v�i kui sa tahad teada, kas mingis failis asub mingi otsitav s�ne? Kindlasti ei hakkaks sa kogu teksti l�bi otsima, sa kasutaksid grep'i!

Kasutame n�itena n�ide.txt faili:

<pre>$ grep rebane n�ide.txt</pre>

Sa peaksid n�gema, et grep leidis s�na rebane failist n�ide.txt

Sa saad ka otsida v�ike- ja suurt�hedele mittetundlikku teksti, kui kasutad lippu -i.

<pre>$ grep -i mingimuster mingifail</pre>

Et veelgi paindlikkust lisada, v�ib grep'i kombineerida teiste k�skudega | operaatoriga.

<pre>$ env | grep -i Kasutaja</pre>

Nagu n�ha, on grep v�ga mitmek�lgne. Mustris v�i kasutada isegi tavap�raseid v�ljendeid:


<pre>$ ls /mingikat | grep '.txt$'</pre>

Peaks kuvama kataloogist mingikat k�ik failid mis l�pevad .txt.

## Harjutus

Ehk oled kuulnud k�skudest egrep ja fgrep, need on n��d vananenud ning asendatud k�skudega grep -E ja grep -F. Loe grep'i man lehek�lge ja saad rohkem teada.

## K�simus

Millist k�sku kasutad, et mingit t�hem�rgi kombinatsiooni leida?

## Vastus

grep
