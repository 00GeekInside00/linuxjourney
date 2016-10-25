# kill (Peatamine)

## Tunni sisu

Protsessi peatamiseks saadetakse signaal, mida nimetatakse *kill*.

<pre>$ kill 12445</pre>

12445 on peatatava protsessi PID. Vaikimisi saadab see TERM signaali. SIGTERM saadetakse aga protsessile, et ta saaks rahulikult oma ressursid vabastada ja staatuse salvestada.

*Kill* k�suga saab signaali ka t�psustada:

<pre>$ kill -9 12445</pre>

See k�ivitab SIGKILL signaali ja peatab protsessi t��.

<b>Erinevused SIGHUP, SIGINT, SIGTERM, SIGKILL, SIGSTOP vahel?</b>

Need signaalid k�lavad k�ik usna sarnaselt, kuid on siiski erinevad.

<ul>
<li>SIGHUP - saadetakse protsessilke kui kontrollterminal on suletud. N�iteks, kui sulgeda terminali aken, milles protsess alles t��tas, siis saadetakse SIGHUP signaal.</li>
<li>SIGINT - See on vahelesegamise signaal. Kui sisestad klahvikombinatsiooni Crtl-C p��ab s�steem graatsiliselt protsessi peatada.</li>
<li>SIGTERM - Peata protsess, aga lase tal enne korralikult enda j�relt �ra koristada</li>
<li>SIGKILL - Peata protsess, peata vahendeid valimata, mingist koristamisest pole juttugi</li>
<li>SIGSTOP - Peatab protsessi ajutiselt </li>
</ul>

## Harjutus

Peatada protsesse erinevate signaalidega.

## K�simus

Milline on vaikimisi peatamise signaal?

## Vastus

SIGTERM

