# Seadmete nimed

## Tunni sisu

M�ned levinumad seadmete nimed:

<b>SCSI seadmed</b>

Massm�luseadmed kasutavad k�ige t�en�olisemalt SCSI (h��ldatakse "skazzi") protokolli. SCSI t�hendab *Small Computer System Interface", mis t�lkes oleks v�ikearvutis�steemi liides. Tegu on protokolliga, mida kasutatakse v�lisseadmete, nagu kettad, printerid, sk�nnerid ja muu, �hendamiseks arvutiga. Eksisteerivad SCSI seadmed, mida kaasajal tegelikult enam ei kasutata, Linux aga samastab SCSI kettad /dev'is k�vaketastega. Neid esindab *sd(SCSI disk):*

Tavap�rased SCSI seadme failid:

<ul>
<li>/dev/sda - Esimene k�vaketas</li>
<li>/dev/sdb - Teine k�vaketas</li>
<li>/dev/sda3 - Esimese k�vaketta kolmas kettajagu</li>
</ul>

<b>Pseudoseadmed</b>

Kordame, et pseudoseadmed ei ole tegeleikult f��siliselt arvutiga �hendatud ning endamik pseudoseadmeid on t�hem�rgi seadmed:

<ul>
<li>/dev/zero - v�tab vastu ja heidab kogu sisendi k�rvale, v�ljundiks on NULL (nullv��rtus) baitide jada</li>
<li>/dev/null - v�tab vastu ja heidab kogu sisendi k�rvale  ning v�ljundit ei anna </li>
<li>/dev/random - toodab juhuslikke numbreid</li>
</ul>

<b>PATA seadmed</b>

M�nikord, just vanemates s�stemides, v�ib n�ha, et k�vaketastele viidatakse hd prefiksiga:

<ul>
<li>/dev/hda - Esimene k�vaketas</li>
<li>/dev/hdd2 - Neljanda k�vaketta teine kettajagu</li>
</ul> 

## Harjutus

Kirjutada pseudoseadmetele, ning uurida v�ljundit. Ettevaatust, et ei krijutaks nendele oma kettaid!

## K�simus

Milline oleks tavaliselt teise SCSI ketta esimese kettajao seadmenimi?

## Vastus

sdb1
