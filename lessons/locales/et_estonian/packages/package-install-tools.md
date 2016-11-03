# rpm ja dpkg

## Tunni sisu

Kuigi suurem osa sellest kurusest r��gib paketihalduss�steemidest (paketihalduse Batmanid), ei tohi unustada ka Robineid. Kuigi v�ga kasulikud ja usaldusv��rsed, ei ole nendel uhket autot ja nutiv��d.

Just nagu .exe on �ksik k�ivitatav fail, on seda ka .deb ja .rpm.Kui kasutada paketihoidlaid, siis tavap�raselt neid eriti ei n�e, kuid kui paketid otse alla laadida, siis on nad nendes poplaarsetes vormingutes. Loomulikult on nad distributsioonip�hised, .deb Debiani ja .rpm Red Hati s�steemidele.

Nende pakettide paigaldamiseks v�ib kasutadak�ske *rpm* ja *dpkg*. N�nda paigaldatakse paketi failid, k�ll aga mitte eelmises peat�kis mainitud olulised s�ltuvused. Seega, kui pektil on 10 s�ltuvust, peaks need paketid ka eraldi veel paigaldama ning sama kehitb omakorda ka nende s�ltuvuste kohta. Nagu isegi n�ha v�ib, on see �ks p�hjusi, mis kutsus ellu t�is kohaga halduss�steemid, millest r��gitakse veidi hiljem.

Kuna ilmselt tuleb ette loendamatu arb kordi kui on vaja nende k�skudega paigaldada, p�rida v�i kinnitada pakette, v�iks need meelde j��ta.

<b>Paketi paigaldamine</b>

<pre>
Debian: $ dpkg -i mingi_deb_pakett.deb
RPM: $ rpm -i mingi_rpm_pakett.rpm
</pre>

*i* t�histab installeerimist ehk paigaldamist. V�ib kasutada ka pikemat formaati --install.

<b>Paketi eemaldamine</b>

<pre>
Debian: $ dpkg -r mingi_deb_pakett.deb
RPM: $ rpm -e mingi_rpm_pakett.rpm
</pre>

Debian: <b>r</b> nagu *remove* t�hendab eemaldamist
RPM: <b>e</b> nagu *erase* t�hendab kustutamist

<b>Kuva paigaldatud paketid</b>

<pre>
Debian: $ dpkg -l
RPM: $ rpm -qa
</pre>

Debian: <b>l</b> nagu loetle
RPM: <b>q</b> nagu *query* ehk p�ring <b>a</b> nagu *all* ehk k�ik

## Harjutus

Leida mingi programm, mida on soov paigaldada, n�iteks Google Chrome, ja paigaldada see kasutades �pitud k�ske.

## K�simus

Milline on .deb failide paketihaldust��riist?

## Vastus

dpkg
