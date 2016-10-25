# Kenadus

## Tunni sisu

Kui tegeleda arvutis mitmete asjadega, korraga on avatud ehk Chrome, MS Word v�i Photoshop, siis v�ib tunduda, et need protsessid t��tavad k�ik samal ajal, kui tegelikult see p�ris nii ei ole.

Protsessid kasutavad protsessorit ainult v�ikese osa ajast, seda nimetatakse time slice. Seej�rel nad peatuvad millsekunditeks ja teised protsessid saavad oma killukese aega. Vaikimis toimub see ikka �ks teise j�rel uuesti ja uuesti. K�ik protsessid saavad piisaalt killukesi aega kuni nad oma t��ga valmis saavad. Tuum haldab kogu seda protsesside �mberl�litumist ja suurem osa ajast teeb seda ka v�ga edukalt.

Protsessid ise ei saa otsustada millal ja kui palju nad protsessori aega kasutada saavad. Kui k�ik t��tavad tavap�raselt, saavad nad k�ik ka (enamv�hem) v�rdselt protsessori aega. On aga v�imalus tuuma protsessi vaikimis algoritmi muutmiseks *nice*(t�lkes kena) v��rtusega. Kenadus on k�ll veider nimi, kuid see t�hendab, et protsessid saavad numbri, mis m��rab nende prioriteedi protsessori jaoks. Suurem number t�hendab, et protsess on kena ja tal on madalam prioriteet protsessori jaoks, v�ike v�i negatiivne number t�hendab, et protsess ei ole v�ga kena ja tahab saada nii palju protsessori aega kui v�imalik.

<pre>$ top</pre>

Tulp NI ongi protsessi kenaduse tase.

Kenaduse taseme muutmiseks v�ib kasutada *nice* ja *renice* k�ske:

<pre>$ nice -n 5 apt upgrade</pre>

*Nice*i kasutatakse uuele protsessile prioriteedi m��ramiseks. *Renice* muudab aga juba olemas oleva protsessi prioriteeti.

<pre>$ renice 10 -p 3245</pre>

## Harjutus

Millised protsessid ei ole eriti kenad ja miks?

## K�simus

Kui on vaja anda protsessile suurem protsessori prioriteet, kas *nice* number peab olema suurem v�i v�iksem?

## Vastus

v�iksem
