# Protsessi detailid

## Tunni sisu

Enne kui s�veneda protsesside praktilise rakendamise poolele, peaks m�istma, mis nad on ja kuidas nad t��tavad. See osa v�ib p�ris keeruliseks minna, kuna l�hme p�ris asja tuumani. Kui pole soovi praegu asjasse s�veneda, v�ib selle peat�ki juurde soovi korral ka hiljem tagasi p��rduda.

Nagu ennegi mainitud on protsess programm, mis s�steemis t��tab, t�psemalt �eldes eraldab s�steem programmile t��tamise jaoks m�lu, protsessorit ja sisendit/v�ljundit. Protsess on t��tava programmi �ks esinemine. Proovida j�rgmist: Avada kolm terminali akent, kahes neist k�iviata <b>cat</b> ilma lippudeta. Kolmandas aknas aga k�ivita <b>ps aux | grep cat</b>. On n�ha kaks *cat*i protessi, hoolimata sellest, et need m�lemad p��rduvad �he programmi poole.

Protsesside eest vastutab tuum. Kui k�ivitada programm, siis tuum laeb m�lust programmi koodi, tuvastab ja m��rab sellele vajalikud ressursid ning peab arvet k�ikide protsesside �le, mis sellega seotud on:

<ul>
<li>Protsessi staatus</li>
<li>Ressursid, mida protsess kasutab ja vastu v�tab</li>
<li>Protsessi omanik</li>
<li>Signal handling (sellest r��gitakse hiljem l�hemalt)</li>
<li>Ja p�him�tteliselt k�ik muu ka</li>
</ul>

K�ik protsessid tahavad maitsta magusad ressursside pirukat, tuuma �lesanne on hoolitseda selle eest, et iga protsess saab just nii palju, kui vaja on. Kui protsess l�ppeb, vabanevad ressursid m�ne teise jaoks.     

## Harjutus

Selles peat�kis harjutust ei ole.

## K�simus

Mis haldab ja kontrollib protsesse?

## Vastus

tuum
