# NFS

## Tunni sisu

K�ite standartsem failide jagamise viis Linuxis on NFS (*Network File System* ehk v�rgu failis�steem). NFS v�imaldab serveril jagada katalooge ja faile �le v�rgu rohkem kui �he kasutajaga.

NFS serveri loomise �ksikasjadesse sellel kursusel ei s��bita kuna see v�ib veidi keeruliseks minna, k�ll aga r��gime NFS kliendi �les seadmisest.

<b>NFS kliendi �les seadmine</b>

<pre>$ sudo service nfsclient start
$ sudo mount server:/kataloog /haagitav_kataloog</pre>

<b>Automaatne haakimine</b>

�tleme, et NFS server on �sna tihti kasutuses ning kasutaja soovib, et see oleks j��davalt k�lge haagitud. Tavaliselt v�iks m�elda, et tuleb muuda /etv/fstab faili, kuid alati ei pruugi �nnestuda saada serveriga �hendust ja see v�ib tekitada alglaadimisel probleeme. Selle asemel tasuks �les seada automaatne haakimine. Seda tehakse <b>automount</b> t��riistaga, uuemates Linuxi versioonides <b>amd</b>. Kui m�nele t�psustatud kataloogile p��takse ligi p��seda otib automount �les vastava serveri ja haagib selle automaatselt k�lge.

## Harjutus

Lugeda NFS'i man-lehek�lge, et selle kohta rohkem teada saada.

## K�simus

Millise t��riistaga hallatakse automaatseid haakepunkte?

## Vastus

automount
