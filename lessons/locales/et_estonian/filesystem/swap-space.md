# Saalimine

## Tunni sisu

Eelmises n�ites tutvustati partitsioonitabelit. Vaatame seda uuesti, aga n��d t�psemalt seda rida:

<pre>
Number  Start   End     Size    Type      File system     Flags
 5      6861MB  7380MB  519MB   logical   linux-swap(v1)
</pre>

Mis on see *swap* ehk saaleala? Saaleala kasutatakse virtuaalm�lule s�steemis ruumi eraldamiseks. Kui m�lumahtu hakkab v�heks j��ma, kasutab s�steem seda kettajagu, et saalida sinna tegevusetute protsesside m�lu "t�kid". N�nda ei saa m�lu otsa.

<b>Kettajao kasutamine saalimiseks</b>

�tleme, et soovime seada oma /dev/sdb2 partitsiooni saalealaks.

<ol>
<li>Esiteks tuleb teha kindlaks, et kettajaol ei asu midagi</li>
<li>K�ivitada: mkswap /dev/sdb2 et inistialiseerida saalealad</li>
<li>K�ivitada: swapon /dev/sdb2 mis lubab saaleseadme</li>
<li>Kui on soovitud, et saalealad p�siksid k�ivitamisel, on vaja lisada ka kirje /etc/fstab faili. Kasutada tuleb sw failis�steemi t��pi.</li>
<li>Saaleala eemaldamiseks: swapoff /dev/sdb2</li>
</ol>

Tavaliselt peaks m��rama kaks korda nii palju ruumi saalealale, kui on m�lu, kuid t�nap�eva s�steemid on juba piisavalt v�imsad, et RAM'ist t�itsa piisab.

# Harjutus

Luua USB pulga vabale alale saaleala.

## K�simus

Millise k�usga lubatakse seadmel saaleala?

## Vastus

swapon