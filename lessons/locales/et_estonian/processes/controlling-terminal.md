# Kontrollterminalid

## Tunni sisu

Eelmises peat�kis sai r��gitud TTY v�ljast *ps*i v�ljundis. TTY on see terminal, mis k�su k�ivitas.

Terminale on kahte sorti: tavap�rased <b>terminalid</b> ja <b>pseudoterminalid</b>. Tavap�rane terminal on kohalik vahend, millesse saab tr�kkida ja saata v�ljund s�steemile. K�lab justnagu terminali raknedus, mida oleme seni kasutanud, et k�ivitada kestaprogrammi, kuid p�ris nii see pole.

Liigume siit n��d sujuvalt edasi, et seda demonstreerida. Kasuta klahvikombinatsiooni Ctrl-Alt-F1, et p��seda ligi virtuaalsele konsoolile TTY1. Kuvatakse ainult terminal, ei mingit graafikat. Seda nimetatakse tavap�raskes terminaliks. Seal saab v�ljuda klahvikombinatsiooniga Ctrl-Alt-F7.

Pseudoterminal on aga juba harjumusp�raseks saanud terminal, mis emuleerib terminali kestaprogrammi aknaga ja m�rgistus on PTS. Kui uuest vaadata *ps*i, siis kasutatav kesta protsess leitav pts/* alt.

Kui n��d ringiga kontrollterminalide juurde tagasi tulla, siis protsessid ongi tavalieslt �hega seotud. N�iteks, kui sul kestaprogrammi aknas mingi protsess t��tab ja see aken sulgeda, siis sulgub koos sellega too protsess.

On olemas spetsiaalsed protsessid, n�iteks deemoni protsessid, mis hoiavad s�steemi k�imas. Need k�ivituav tavaliselt s�steemi alglaadimisel ja peatuvad kui s�steem v�lja l�litada. Need protsessid t��tavad taustal ja kuna me ei taha, et need peatuksid, siis ei ole need ka �hegi kontrollterminaliga seotud. *ps*i v�ljundis on TTY koha peal ?, mis t�hendabki, et kontrollterminal puudub. 

## Harjutus

Vaadata *ps*i v�ljundit ja t�heldada k�iki unikaalseid TTY v��rtusi.

## K�simus

Milline v��rtus antakse protsessile, millel ei ole kontrollterminali?

## Vastus

?
