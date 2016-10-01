# env (Environment)

## Tunni sisu

K�ivita k�sk:

$ echo $HOME

Sa peaksid n�gema oma kodukataloogi otsiteeknda, minu oma n�eb selline v�lja /home/pete.

Aga see k�sk?

$ echo $USER 

Sa peaksid n�gema enda kasutajanime!

Kust see infiormatsioon p�rineb? See p�rineb sinu keskkonna muutujatest. Sa saad neid n�ha, kui tr�kid

$ env 

See v�ljund, kuvab palju infot selle kohta, millised keskkonna muutujad sul parasjagu seatud on. Nendes muutujates on palju kaslikku infot, mida kest ja teised protsessid saavad kasutada.

Siin on l�hike n�ide:

<pre>
PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/bin
PWD=/home/user
USER=pete
</pre>

�ks eriliselt oluline muutuja on PATH muutuja.  Nendele saab ligi, kui topid $ s�mboli muutujanime ette, niimoodi:

<pre>
$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/bin
</pre>

See tagastab nimekirja koolonitega eraldatud teekondades, milleni su s�steem ulatub, kui see k�ivitab k�su.  �tleme, et sa laed Internetis k�sitsi alla ja paigaldad paketi, mille sa paned mittestandardsesse kataloogi ja tahas k�ivitada k�sku. Sa kirjutad $ lahek�sk ja k�suviip �tleb, et k�sku ei leitud. See on k�ll tobe. Sa vaatad kaustas binaari ja tead, et see on olemas. Mis toimub on see, et  $PATH muutuja ei kontrolli selle kataloogi seda binaari ning seet�ttu annab veateate.

�tleme, et sul on tonnides binaare, mida sa tahad k�ivitada v�ljaspool seda kataloogi, sa v�id lihtsalt muuta PATH muutujat, et see sisaldaks vajalikku kataloogi sinu PATH keskkonna muutujas.

## Harjutus

Mida teeb j�rgmine k�sk? Miks?
<pre>$ echo $HOME</pre>

## K�simus

Kuidas sa n�ed keskkonna muutujaid?

## Vastus

env

