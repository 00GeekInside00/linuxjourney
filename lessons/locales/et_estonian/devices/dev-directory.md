# /dev kataloog

## Tunni sisu

Seadmed vajavad arvutisse �hendamisel tavaliselt juhtprogramme, et korralikult t��tada. Seadmete juhtporgrammidega saab tegeleda l�bi seadme failide v�i seadmes�lmede, mis on tegelikult lihtsalt erilised failid, mis n�evad v�lja nagu tavalised failid. Kuna seadme failid on just nagu tavalised failid, saab nendega tegutsemiseks kasutada programme nagu *ls*, *cat* jne. Seadmete faile hoitakse tavaliselt kataloogis /dev. Kui sisestada *ls* /dev kataloogis, v�ib n�ha suurt hulka erinevaid seadmefaile.

<pre>$ ls /dev </pre>

M�nda seadet on siin kursustel juba kasutatud ka, n�iteks /dev/null. �hes peat�kis sai /dev/null'le saadetud v�ljund, tuum teab rakendada seda seadet ja lihtsalt heita sisend k�rvale, v�ljundit ei tagastata.

Kui vanasti taheti lisada s�steemi seadmeid, v�is lihtsalt lisada faili /dev kataloogi ja ta sinna unustada. Kui n��d h�sti j�rgi m�elda, siis taipab peagi, miks see ei ole eriti hea m�te. /dev kaust kuhjub t�is staatilisi faile v�i seadmeid, mida on juba ammu uunedatud, kasutamine l�petatud vms. Seadmetele m��ratakse seadmefail selles j�rjekorras, milles tuum nad leiab. Nii v�is juhtuda, et iga kord kui s�steem taask�ivitada, on seadmel erinev seadmefail.

�nneks enam sellist meetodit ei kasutata. N��d kasutame midagi, et lisada ja eemaldada seadmeid d�naamiliselt ja sellest r��gitakse tulevates peat�kkides.

## Harjutus

Uurida /dev kasuta sisu. Kas on m�rgata tuttavaid seadmeid?

## K�simus

Kus hoitakse s�steemi seadmefaile?

## Vastus

/dev
