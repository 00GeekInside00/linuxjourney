# Juur

## Tunni sisu

Eelmises peat�kis vaadeldi �hte superkasutajale ligip��semise viisi. Superkasutaja k�ske saab sisestada ka *su* k�suga. See k�sk vahetab kasutaja v�lja, kui kasutajanime ei t�psustata, avab see k�sk kestaprogrammi juur�igustes. Selle k�suga saab vahetada kasutajat �ksk�ik millise vastu, vaja on ainult teada ka vastavat parooli.

<pre>$ su</pre>

Eks sellel metoodikal on ka pahupool: juurkasutajana t��tades on palju lihtsam on teha kriitilisi vigu. N�iteks, ei peata arvet nende k�skude �le, mida kasutatakse s�steemi seadete muutmiseks jpm. Lihtsamalt �eldes, kui on vaja sisestada k�sku superkasutajana, tasub esialgu j��da *sudo* juurde.

N��d on selge kuidas sisestada k�ske superkasutajana. Kuid kuidas teha kindlaks, kellel on selleks �igused? S�steem ei lase igal Tuha Juhanil superkasutajana k�ske sisestada. Kuidas ta siis aga teab? On olemas fail /etc/sudoers, milles on nimekiri kasutajatest kellel on �igus *sudo*t kasutada. Seda faili saab muuta k�suga <b>visudo</b>.

## Harjutus

Avada /etc/sudoers fail ja vaadata milliseid superkasutaja �igusei teistel kasutajatel selles masinas on.

## K�simus

Millisest failist saab infot selle kohta, kellel on ligip��su �igus *sudo*le?

## Vastus

/etc/sudoers
