# Tarkvarahoidlad

## Tunni sisu

Kuidas saavad Internetti �leslaetud pakettid �ht�kki kasutajate arvutitesse? Kas peab minema igapaketti lehek�ljele ja laadima nad alla ja paigaldama? Tegelikult v�ib seda muidugi ka nii teha, kuid on olemas palju parem lahendus, mida nimetatakse paketihoidlateks. Need ongi lihtsalt kesksed hoidlad pakettide jaoks. On olemas palju hoidlad, mis hoiavad palju pakette ja mis k�ige parem, need on k�ik ka Internetist leitavad, mis t�hendab, et tobedaid paigaldamiskettaid pole �ldse tarvis. K�ll aga ei oska arvutid ise ilma kasutaja abita neid hoidlaid otsida.

N�iteks, �tleme, et kasutaja soovib oma arvutisse WackyWidgets tarkvara. WackyWidgets haldab ise enda pakettide hoidlaid. Hoidlates on 10 pakettid: CoolWidget, SuperWidget jne. WackyWidget hoiab oma hoidlat aadressil http://download.widgets/linux/deb/.

Selle asemel, et minna veebilehele pakette allalaadima, v�ib �elda arvutile, kust tarkvara leida.

Operatsioonis�steemi distributsioonidiel on juba algselt mingisugesed heaks kiidetud allikad, kust s�steem saab peamised olulised pakettid. Debiani puhul on selleks failiks <b>/etc/apt/sources.list</b>. Arvuti oskab otsida sealt erinevaid allikaid, sealjuures neid, mida kasutajad v�ivad olla lisanud.

## Harjutus

Selles peat�kis harjutus ei ole.

## K�simus

Kus asub Debiani s�steemis l�htefail?

## Vastus

/etc/apt/sources.list
