# /etc/passwd

## Tunni sisu

Meenutame, et kasutajanimed ei ole tekelikult kasutajate tuvastamise aluseks. S�steem kasutab selleks hoopis kasutajate IDsid (UID). Selleks, et n�ha millised kasutajad milliste IDdega seotud on, v�ib vaadata faili /etc/passwd.

<pre>$ cat /etc/passwd</pre>

See fail sisaldab nimekirja kasutajatest ja iga�he kohta ka detailset informatsiooni. N�iteks, k�ige t�en�olisemalt n�eb faili esimene rida v�lja n�nda:

<pre>root:x:0:0:root:/root:/bin/bash</pre>

Iga rida kuvab infot �he kasutaja kohta ning juurkasutaja on tavaliselt k�ige esimesel real. Paljud koolonitega eraldatud v�ljad annavad kasutajate kohta t�iendavat infot, vaatame neid k�iki:

<ol>
<li>Kasutajanimi</li>
<li>Kasutaja parool - parooli ennast tegelikult selles failis ei hoita, tavaliselt on see hoopis failis /etc/shadow. Sellest failist r��gitakse rohkem j�rgmises peat�kis, praegu aga v�iks meelde j�tta vaid, et seal hoitakse kasutajate kr�pteeritud parole. Selles v�ljas v�ivad olla v�ga erinevad s�mbolid. "x" t�hendab, et parooli hoitakse failis /etc/shadow, "*" t�hendab, et kasutajal puudub sisse logimise �igus ja kui see v�li on t�hi, t�hendab, et kasutajale pole parooli seatud.</li>
<li>Kasutaja ID - nagu n�ha on juurkasutaja UID 0</li>
<li>Grupi ID</li>
<li>GECOS v�li - Tavap�raselt kasutatakse seda v�lja, et j�tta kasutaja konto kohta kommentaar, n�iteks kasutaja p�ris nimi v�i telefoni number, eraldajaks on koma.</li>
<li>Kasutaja kodukataloog</li>
<li>Kasutaja kestaprogramm - v�ga paljudel kasutajatel on see vaikimisi *bash*</li>
</ol>

Tavaliselt oleks ootusp�rane leida kasutaja seadete lehelt vaid inimkasutajad, siin aga on n�ha, et /etc/passwd sisaldab ka teisi. Meenutame, et kasutajad eksisteerivad ainult selleks, et s�steemis erinevate �igustega protsesse k�ivitada. M�nikord on eelistatud k�ivitada mingeid protessse eelnevalt s�testatud �igustest. N�iteks, deemoni kasutajat kasutatakse deemoni protseside jaoks.

M�rgiks �ra, et  /etc/passwd faili saab ka k�sitsi muuta, kui on vaja lisada kasutajaid v�i muuta olemasolevate informatsiooni. Selleks on t��riist nimega <b>vipw</b>, kuid targem oleks siisi j�tta sellised tegevused t��riistadele, millest r��gitakse veidi hiljem. Need on n�iteks *useradd* ja *userdel*. 

## Harjutus

Vaadata faili /etc/passwd ning uurida milliseid �igusi erinevatel kasutajatel on.

## K�simus

Kuidas on m�rgitud failis /etc/passwd, kui kasutajal puudub sisselogimise �igus?

## Vastus

*
