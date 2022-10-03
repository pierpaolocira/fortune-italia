# fortune-italia (work in progress)
**In breve:** questo repository vorrebbe essere una versione sempre aggiornata dalla comunità del database ufficiale dei fortune. Facciamolo crescere insieme!!!

Quindi attenzione: stiamo parlando solo del database e non dei player, che saranno dei progetti a parte.

## Breve storia

Tutto iniziò con i *fortune*: si tratta dell'equivalente informatico dei biscottini della fortuna (approfondimenti alla [voce "Fortune" di Wikipedia](https://en.wikipedia.org/wiki/Fortune_%28Unix%29#Purpose)).

Dal 1998 al 2004 (e sì, è passato tanto tempo) *Mirko Caserta* inizialmente e poi *Andrea 'Zuse' Balestrero* hanno manutenuto una versione italiana del database dei file *fortune*, reperibile presso [http://www.fortune-it.net/main.html](http://www.fortune-it.net/main.html) insieme a tutte le informazioni del caso.

## L'idea di questo repository
Essendomi divertito non poco con i fortune, e poi avendo scoperto quelli in italiano, mi sono rattristato non poco a vedere che il pacchetto *fortune-it* non era più aggiornato da quasi 12 anni *[dal sito fortune-it.net: «ultimo aggiornamento a queste pagine o al package fortune-it qui contenuto: venerdì 3 dicembre 2004»]*.

Quello che mi sarebbe piaciuto vedere, in quest'era in cui anche scrivere dei progetti software può diventare un'operazione sociale, è un aggiornamento costante di questo pacchetto fatto da chiunque avesse avuto il piacere di contribuire in maniera intelligente e costruttiva.

Come da indicazioni nel package originale, ho provato a contattare *Andrea Balestrero* il *28 marzo 2016*, per capire se potevamo provare insieme a rendere sociale *fortune.it*.

Il *18 settembre 2016* mi ha risposto
> Ciao.
> Hai pieno margine di manovra su tutto cio' che vuoi.
> Io cedero' il progetto a chi potra' seguirlo, perche'
> io non ho piu' tempo di starci dietro...
> Licenza: fa' cio' che vuoi, purche' citi chi ci ha lavorato prima.
> Bau,
>          (very late) Zuse

E ci mancherebbe altro, dopo l'enorme lavoro fatto prima di noi che andiamo solo in aggiunta. Per citare Bernardo di Chartres: "siamo nani sulle spalle dei giganti": il nostro sguardo va più avanti, solo grazie a chi ci ha preceduto!

A proposito di licenza: dal file *COPYING* del package originale (che consiglio comunque di leggere): «Considerate freeware (public domain) questo package» e dal file *lsm*: «Copying-policy:	Freeware».

## Il futuro?
Per il futuro vorrei che questa mia idea portasse il pacchetto a crescere e attualizzarsi costantemente grazie all'aiuto di tutti voi.

Se l'idea vi piace, fate un fork del repository, aggiungete tutto quello che volete, e fate una "pull request": lavoriamo insieme per tenere un'unico repository il più aggiornato possibile.

Mi piacerebbe anche che fungesse da "spinta" per la realizzazione di nuovi player di *fortune* per varie piattaforme, magari in grado di *autoaggiornarsi* con le versioni, sempre più recenti, dei file di database che saranno qui pubblicati.

## Nota: come funzionano i player di database Fortune?

Fortune nasca come un programma a riga di comando che estrae una frase a caso da un file. Esempio

    fortune
      
     Dio ha creato i numeri interi; tutto il resto e' lavoro dell'Uomo. 
     - Kronecker, matematico tedesco  

Per aggiungere delle frasi o eliminare altre (ma con questa andateci cauti), basta andare nella directory di fortune (di solito **/usr/share/fortune/** e vedere se e' presente una directory chiamata **"fortunes"**, se non c'e' createla. A questo punto spostate tutti i file di testo e .dat in quest'ultima directory appena creata.

I file di testo contengono le frasi estratte a caso dal programma, ogni frase e' separata dal simbolo %. Per aggiungere una frase basta aggiungerlo in uno dei file di testo e similmente per cancellarlo basta eliminarlo. Ogni file modificato va indicizzato per essere utilizzato, e va usato il comando strfile, esempio:

     strfile barzellette 

Si possono usare piu' file di testo, poiché e' possibile indicare a fortune se utlizzare solo una specifica lista, inoltre è possibile indicare con che probabilita' deve esere scelto un file tra i vari file.

     fortune 90% barzellette 10% barzellettesporche

## Responsabilità dei contenuti
La serie iniziale di *fortune* appartiene a un periodo storico in cui il concetto di "politicamente corretto" aveva un'accezione molto diversa da quella attuale.

Senza voler entrare nel merito della questione è importante sottolineare che **il gestore di questo repository non è da considerarsi in alcun modo responsabile dei contenuti qui presenti e questi non devono essere in alcun modo collegati alla sua opinione personale e/o professionale.**

In generale, nessuno dovrebbe essere ritenuto responsabile per una frase che ha il solo scopo di far divertire (anche se non ci riesce), soprattutto se questa non vuole essere altro che una battuta fine a sé stessa e non vuole avere impatto di alcun tipo sulla vita di nessuno (se non quello di strappare un sorriso istantaneo).
**Chiunque fornisca nuovo materiale per questo repository lo fa accettando implicitamente che non vuole fare nulla di diverso da quanto appena specificato.**

Qualora rinveniate un *fortune* che ritenete offensivo in qualsiasi forma, siete pregati di proporre una "pull request" contenente la modifica desiderata e la relativa motivazione.
A tal proposito vorrei specificare che **sarebbe corretto trattare questo repository anche come un archivio storico e, pertanto, conservare il maggior numero di contenuti esistenti dal momento il cui i fortune italiani sono stati importati qui**

Sarebbe fantastico se questo repository prendesse vita con una board di persone in grado di definire delle linee guida sui contenuti e valutare democraticamente qualsiasi pull request in arrivo.
