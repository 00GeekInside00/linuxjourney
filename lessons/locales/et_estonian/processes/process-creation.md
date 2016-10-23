# Protsesside loomine

## Tunni sisu

See ja eelmine peat�kk on puhtalt informatiivsed, et tutvustada natuke kapotialust. V�id igal ajal siia tagasi p��rduda, kui oled juba veidi rohkem protsesside kallal t��tanud.

Protsessi loomisel p�him�tteliselt kloonitakse juba olemasolevat protsessi kasutades midagi, mida nimetatakse *fork* s�steemseks kutseks (s�steemsetest kutsetest r��gitakse alles v�ga kauges tulevikus). *Fork* kutse loob olmeasolevale protsessile identse t�tarprotsessi, mis v�tab endale uue protsessi ID (PID) ja esialgsest protsessist saab emaprotsess, mis saab endale emaprotsessi ID <b>PPID</b>. Hiljem v�ib aga t�tarprotsess j�tkata sama programmi kastuamist, mida kasutas tema ema v�i kasutada *execve* s�steemset kutset, et k�ivitada uus programm. See kutse h�vitab senise tuuma poolt selle protsessi jaoks loodud m�lu haldamise ning seab �les uued just selle programmi jaoks.

Seda v�ib tegevuses n�ha:

<pre>$ ps l</pre>

Valik l (nagu *long format* ehk pikk formaat) v�imaldab jooksvaid protsesse vaadeleda isegi veel detailsemalt. N�ha on tulp nimega <b>PPID</b>, see ongi ema ID. Kui n��d vaadata oma terminali, siis on n�ha protsess, mis on jooksev kestaprogramm, n�iteks *bash*. Meenuta, et kui sisestasid *ps l* k�su, k�ivitasid sa selle protsessist, mis k�itas *bash*i. M�rka, et *bash*i kesta <b>PID</b> on selle *ps l* k�su <b>PPID</b>.

Seega, kui igal protsessil peab olema ema ja k�ik protsessid on �ksteise harud, peab ju kusagil olema k�ikide protsesside ema, eks? Nii ongi. Kui s�steem algk�ivitub, loob tuum protsessi nimega <b>init</b>, mille PID on 1. Seda protsessi saab peatada vaid siis kui s�steem v�lja l�litada. *Init* jookseb juurkasutaja �igustes ja k�itab mitmeid teisi protsesse, mis v�imaldavad s�steemil t��tada. *Init* tuleb l�hema vaatluse alla s�steemi algk�ivitamise kursusel, praegu v�iks meelde j�tta, et tegu on k�ikide teiste protsesside loojaga.

## Harjutus

Kui vaadata t��tavaid protsesse, millistel protsessidel veel on emad?

## K�simus

Milline s�steemi kutse loob uue protsessi?

## Vastus

fork
