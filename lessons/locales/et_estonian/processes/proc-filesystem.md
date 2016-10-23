# /proc failis�steem

## Tunni sisu

Meenutame, et Linuxis on k�ik asjad failid, isegi protsessid. Informatsiooni protsesside kohta hoitakse spetsiaalses failis�steemis /proc.

<pre>$ ls /proc</pre>

Sealt paistavad erinevad v��rtused, iga PID jaoks on alamkataloog. Kui eelnevalt on *ps* v�ljundi abil PID tuvastatud, saab selle /proc kaustast �les otsida.

Sisestame �he protsessi ja uurime selle faili:

<pre>$ cat /proc/12345/status</pre>

Seal on informatsioon staatuse kohta, aga ka palju muud detailset infot. Tuum n�eb s�steemi nii nagu see on /proc kaustas, mist�ttu on seal ka oluliselt rohkem infot kui *ps* n�itab.

## Harjutus

Selles peat�kis harjutust pole.

## K�simus

Millises failis�steemis hoitakse infot protsesside kohta?

## Vastus

/proc
