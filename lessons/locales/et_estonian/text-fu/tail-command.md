# tail

## Tunni sisu

Sarnaselt head k�suga, laseb tail k�sk sul vaadata vaikimis mingi faili viimast 10 rida.

<pre>$ tail /var/log/syslog</pre>

Just nagu head puhulgi, saad sa muuta, mitu rida kuvatakse.

<pre>$ tail -n 10 /var/log/syslog</pre>

Teine hea variant on kasutada -f (inglise keeles follow ehk j�rgi) lippu. See j�rgib faili, kui see peaks kasvama. Proovi ja vaata, mis juhtub.

<pre>$ tail -f /var/log/syslog</pre>

Kui sa kasutad oma s�steemi, muutub su syslog fail pidevalt. Tail -f k�su kasutamisega n�ed sa k�ike, mida sinna faili parasjagu lisatakse.

## Harjutus

Vaata tail k�su man lehek�lge ja uuri m�ne k�su kohta, mida me ei tutvustanud.

<pre>$ man tail</pre>

## K�simus

Millist lippu kasutakse faili jooksvaks j�lgimiseks?

## Vastus

-f
