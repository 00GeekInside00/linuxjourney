# stderr (Standard Error)

## Tunni sisu

Proovime n��d midagi natuke teistsugust. Proovime saada sisu loetelu mingist kataloogist, mida ei eksisteeri ja suuname selle info taaskord p�hklid.txt faili.

<pre>$ ls /olematu/kataloog > p�hklid.txt </pre>

Sa peaksid n�gema midagi sellist:

<pre>ls: cannot access /fake/directory: No such file or directory</pre>

Ehk sa m�tled, kas see teade ei oleks pidanud saadetama hoopis faili? Tegelikult on olemas veel �ks sisend-v�ljundvoog, standardveav�ljund (stderr). Vaikimisi saadab stderr oma v�ljundi muuhulgas a ekraanile, see on stdout voost t�iesti erinev ja selle v�ljundit tuleb ka suunata teisiti.

Kahjuks ei ole see �mbersuunamise operaator sama kena, kui <b>&lt;</b> v�i <b>&gt;</b>, kuid see on �sna sarnane. Me peake kasutama failideskriptorit.  Failideskriptor on mittenegatiivne number, mida kasutatake, et faili voole ligi p��seda. Me s��bime sellesse hiljem, kuid praegu pead sa teadma, et failideskriptor stdin, stdout ja stderr jaoks on vastavalt 0, 1 ja 2.

Seega, kui me tahame suunata oma stderr �mber faili, saame me toimida j�rgnevalt:

<pre>$ ls /olematu/kataloog 2> p�hklid.txt</pre>

Sa peaksid n�gama failis p�hklid.txt ainult stderr teadet.

Aga mis saab siis, kui ma tahan n�ha nii stderr kui ka stdout v�ljundit p�hklid.txt failis?s Seda saab samuti teha failideskriptoriga:

<pre>$ ls /olematu/kataloog > p�hklid.txt 2>&1</pre>

See k�sk saadab ls /olematu/kataloog tulemuse failile p�hklid.txt ja seej�rel suunab stderr v�ljundi stdout'le kasutades operaatorit 2>&1. Siin on oluline toimingute j�rjekord, 2>&1 saadab stderr'i millelegi, millele stdout viitab. Hetkel viitab see failile. Seega, kui sa avad selle p�hklid.txt faili, pekasid sa n�gema m�lemat, stderr ja stdout v�ljundit. Meie n�ite p�hjal, on �lemise k�su v�ljund ainult stderr.

Selline on l�hem viis, kuidas suunata m�lemad, stdout ja stderr, faili:

<pre>$ ls /olematu/kataloog &> p�hklid.txt</pre>

Aga mis siis, kui ma ei tahagi seda �leliia risustavat infot ja tahan stderr teadetest t�ielikult vabaneda? Sa v�id suunata v�ljundi spetsiaalsesse faili /dev/null ja igasugune sisendinfo lihtsalt heidetakse k�rvale.

<pre>$ ls /olematu/kataloog 2> /dev/null</pre>

## Harjutus

Mida teeb allolev k�sk?

<pre>$ ls /olematu/kataloog >> /dev/null 2>&1</pre>

## K�simus

Millist m�rki kasutatakse stderr �mbersuunamiseks?

## Vastus

2>
