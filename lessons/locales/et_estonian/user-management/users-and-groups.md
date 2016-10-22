# Kasutajad ja grupid

## Tunni sisu

Traditsiooniliselt on igas operatsioonis�steemis kasutajad ja grupid. Need eksisteerivad selleks, et tagada ligip��su ja �igusi. Iga protsess k�ivitub selle omaniku �igustes, olgu see siis Mari v�i Mart. Failide ligip��s ja omandus s�ltub samuti ligip��su �igustest. Me ju ei taha, et Mari n�eks Mardi dokumente ja vastupidi.

Igal kasutajal on isiklik kodukataloog, kus hoitakse kasutajaga seotud faile. See asub tavaliselt /home/kasutajanimi, kuid v�ib distributsiooniti erineda.

S�steem kasutab kasutajate haldamiseks kasutaja IDsid (UID), kasutajanimed on s�bralikum viis kasutaja tuvastamiseks, kuid s�steem kasutab sellkes just UIDsid. Sellele lisaks on s�steemis �iguste haldamiseks grupid, mis kujutavad endast lihtsalt mingit komplekti kasutajaid, kellel k�igil on samad grupi �igused. Neid eristatakse s�steemis grupi ID (GID) j�rgi.

Linuxis v�ivad olla ka kasutajad, kes ei olegi tavap�rased s�steemi kasutavad inimesed. Leidub selliseid kasutajaid, kes on tegelikult s�steemi deemonid, mis �idevalt jooksutavad protsesse ja hoiavad s�steemi t��korras. �ks olulisimaid selliseid kasutajaid on juur v�i superkasutaja. Juurkasutaja on s�steemis k�ige m�juv�imsam, ta saab ligi k�ikidele failidele ja k�ivitada v�i peatada �ksk�ik millist protsessi. Sellel p�hjusel on ka ohtlik pidevalt juurkasutajana tegutseda, v�ib n�iteks kogemata kustutada m�ne kriitilise s�steemi faili. �nneks aga, kui kasutajal on ligip��s juurele ja tal selle �igusi peaks vaja minema, v�ib ta sudo k�suga sisestada k�ske hoopis juurkasutaja �igustega. Sudo k�sku (*superuser do*) kasutataksegi just selleks, et k�sk k�ivituks juure �igustega. Sellest, kuidas kasutaja saab omandada juurkasutaja �igsued r��gitakse s�vitsi veidi hiljem.

Proovi vaadata kaitsud faili, n�itks /etc/shadow:

<pre>$ cat /etc/shadow</pre>

Pane t�hele, et antakse veateade ligip��su keelamise kohta. Nii saab vaadata �igusi:

<pre>$ ls -la /etc/shadow

-rw-r----- 1 root shadow 1134 Dec 1 11:45 /etc/shadow
</pre>

�igustest ei ole k�ll veel l�hemalt r��gitud, kuid eelnevast on n�ha, et faili omanik on juur (ehk *root*) ja faili sisu lugemiseks on vaja juurkasutaja ligip��su�igusi v�i kuulumist *shadow* gruppi. N��d aga prooviks sama k�sku *sudo*ga:

<pre>$ sudo cat /etc/shadow</pre>

N��d on faili sisu n�htav!

## Harjutus

Selles peat�kkis harjutust ei ole.

## K�simus

Kuidas saab sisestada k�sku juurkasutaja �igustega?

## Vastus

sudo
