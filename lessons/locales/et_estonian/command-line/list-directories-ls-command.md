# ls (List Directories)

## Tunni sisu

N��d, kus me oskame s�steemis ringi liikuda, kuidas saaksime teada, kuhu meil �ldse on v�imalik minna? Hetkel me ekleksime justkui pimeduses. Meil on v�imalik kasutada imelist ls k�sku, et kuvada kataloogide sisu. Ls k�sk kuvab vaikimisi k�ik jooksvas kataloogis asuvad kataloogid ja failid, kuid v�id ka t�psustada, millise asukoha sisu sa n�ha soovid.

<pre>$ ls
$ ls /home/pete</pre>

ls on p�ris kasulik t��riist, sest see n�itab sulle kuvatud failide ja kataloogide kohta detailset informatsiooni.

Pea meeles, et mitte k�ik failid ja katalookig ei ole sulle n�htavad. Failid, mille nimed algavad . on peidetud, kuid neid saab n�ha ls k�suga kui sellele on lisatud lipp -a (inglise keeles a nagu all ehk k�ik).

<pre>$ ls -a</pre>

�ks kasulik lipp on veel, -l nagu long ehk pikk. See kuvab failide detailse nimekirja pikemas formaadis. Detailne info, mida kuvatakse on alates vasakult: faili �igused, �henduste arv, omaniku nimi, omanik-grupp, faili suurus, viimase muutmise ajatempel, ja faili/kataloogi nimi.

<pre>$ ls -l</pre>

<pre>pete@icebox:~$ ls -l
total 80
drwxr-x--- 7 pete penguingroup   4096 Nov 20 16:37 T��laud
drwxr-x--- 2 pete penguingroup   4096 Oct 19 10:46  Dokumendid
drwxr-x--- 4 pete penguingroup   4096 Nov 20 09:30 Allalaadimised
drwxr-x--- 2 pete penguingroup   4096 Oct  7 13:13   Muusika
drwxr-x--- 2 pete penguingroup   4096 Sep 21 14:02 Pildid
drwxr-x--- 2 pete penguingroup   4096 Jul 27 12:41   Avalik
drwxr-x--- 2 pete penguingroup   4096 Jul 27 12:41   Mallid
drwxr-x--- 2 pete penguingroup   4096 Jul 27 12:41   Videod</pre>

K�skudel on funktsionaalsuse lisamiseks lipud (v�i argumendid v�i valikud, kuidas sulle parasjagu meeldib neid nimetada).  M�rkasid, et lisasime -a ja -l, neid saab ka koos kasutada, lisades k�sule -la. Lippude j�rjekorrast oleneb, mis j�rjekorras k�ksu t�idetakse. Enamus ajast ei ole sellel erilist t�hendust, nii et v�id kirjutada ka -al ja see t��tab sellegi poolest.

<pre>$ ls -la</pre>

## Harjutus

Proovi sisestada ls k�sku erinevate lippudega ja vaata, mis v�ljundi sa saad.

## K�simus

Millist k�sku sa kasutaksid, et n�ha peidetud faile?

## Vastust

ls -a