# paste

## Tunni sisu

Paste k�sk on sarnane cat k�sule. See �hendab read failis kokku.
Loome uue faili j�rgneva sisuga:

<pre>
n�ide2.txt
kiire
pruun
rebane
</pre>

�hendame n��d k�ik need read:

<pre>$ paste -s n�ide2.txt</pre>

Vaikimisi on paste'i eraldaja tabulaator, seega n��d on siis �ks rida, kus iga s�na eraldab tabulaator.

Muudame selle eraldaja (-d) millegi loetavama vastu:


<pre>$ paste -d ' ' -s n�ide2.txt</pre> 

N��d peaks k�ik olema �hest reas eraldatuna t�hikute poolt.

## Harjutus

Proovi paste k�sku mitme faili peal, mis juhtub?

## K�simus

Millist lippu sa kasutad, et saada kogu sisu �hele reale?

## Vastus

-s
