---
title: Dal Suono ai numeri – Un viaggio unplugged nel digitale
author: Fabio Viggiano
date: 19/05/2025
---

Esame di Didattica dell'Informatica - A.A. 2024/2025

# Inquadramento del lavoro

## Livello di scuola, classe/i, indirizzo

L' unità didattica si rivolge alla scuola secondaria di I grado (scuole medie) dunque studenti e studentesse di età compresa tra gli 11 ed i 13/14 anni. L' informatica, che è la disciplina prevalente, si integra con tecnologia (processi di trasformazione), matematica (grafici cartesiani, approssimazione), scienze (onde sonore) e musica (natura del suono).

Questa unità didattica può essere adattata sia verso studenti di età inferiore che superiore, in tal modo:

**Scuola Primaria (classi 4-5):** Semplificando ulteriormente la terminologia, usando griglie più grandi e meno livelli di quantizzazione, concentrandosi sull'idea di "fare foto" (campionare) e "arrotondare" (quantizzare) un disegno.

**Scuola Secondaria di II grado (primo biennio):** Introducendo concetti più formali come frequenza di campionamento (Hz), bit depth, teorema di Nyquist (in modo intuitivo), e discutendo maggiormente il trade-off qualità/dimensione file.

## Motivazione e finalità

La presente attività si inserisce all’interno del percorso di educazione scientifica e tecnologica della scuola secondaria di I grado, con l’obiettivo di introdurre concetti fondamentali dell’informatica in modo intuitivo e concreto. In particolare, si affronta il tema della digitalizzazione del suono, un argomento di grande attualità e rilevanza, spesso trascurato nei programmi scolastici.
L’attività è progettata per essere unplugged, ovvero priva di strumenti tecnologici complessi, al fine di stimolare la comprensione profonda dei concetti attraverso la manipolazione diretta e la simulazione analogica dei processi di campionamento e quantizzazione.

### Obiettivo generale

Accompagnare gli studenti della scuola secondaria di primo grado alla scoperta del mondo digitale attraverso attività unplugged legate al suono, favorendo la comprensione dei concetti di campionamento, quantizzazione, e rappresentazione numerica del suono.

### Obiettivi Specifici

**Area: Tecnologia / Informatica**

Comprendere che i dispositivi digitali rappresentano i suoni attraverso numeri.

Intuire i concetti base di analogico vs digitale.

Conoscere il processo di campionamento (trasformazione di un segnale continuo in una sequenza discreta).

Conoscere il processo di quantizzazione (approssimazione del valore di ciascun campione a un insieme finito di valori).

Rappresentare graficamente un suono semplificato su carta millimetrata e convertirlo in valori numerici.

Riflettere sui limiti e le approssimazioni della digitalizzazione del suono.

**Area: Matematica**

Usare il piano cartesiano per rappresentare graficamente funzioni semplici.

Saper leggere e scrivere coordinate (tempo, ampiezza).

Comprendere il significato di “intervallo”, “scala”, “valore medio”, “errore di approssimazione”.

Applicare semplici trasformazioni numeriche (arrotondamenti, troncamenti).

**Area: Educazione Civica / Competenze digitali**

Comprendere che il digitale è costruito su astrazioni e scelte progettuali.

Sviluppare il pensiero computazionale attraverso la rappresentazione di dati.

Acquisire consapevolezza del ruolo della digitalizzazione nella vita quotidiana (es. musica digitale, telefonia, videochiamate).

**Competenze trasversali**

Competenze Trasversali

- Collaborazione: lavorare in gruppo per analizzare e trasformare il suono.

- Problem solving: risolvere situazioni didattiche attraverso modelli.

- Pensiero critico: riflettere sulle differenze tra mondo analogico e digitale.

- Comunicazione: raccontare in modo efficace ciò che si è fatto (es. presentazione finale dell’attività).

## Innovatività

Sebbene le attività unplugged per l'informatica siano diffuse, questa proposta si focalizza specificamente sulla visualizzazione manuale e combinata del campionamento e della quantizzazione su carta millimetrata come processo sequenziale applicato a un segnale disegnato dagli studenti stessi. L'approccio manuale rende più chiari i passaggi e l'approssimazione necessaria, cosa che le simulazioni software fanno meno.

Esistono risorse online e attività unplugged generiche sulla rappresentazione binaria. CS Unplugged ha attività sulla rappresentazione delle immagini, ma meno focalizzate sul processo A/D audio in questo modo specifico. Questa unità:

Mantiene: L'approccio unplugged e l'uso di metafore concrete.

Differenzia/Migliora: Integra campionamento e quantizzazione in un unico flusso di lavoro manuale, partendo da un "segnale" creato dallo studente, rendendo il processo più personale e tangibile. Enfatizza la visualizzazione della perdita di informazione confrontando il disegno originale con quello "digitalizzato".

L' innovatività della lezione in questione è quindi presente come lo studente creatore del segnale, quindi protagonista del processo. La digitalizzazione avviene fisicamente, passo-passo, su carta, rendendo visibile e modificabile ogni singolo passo della conversione A/D; a ciò si aggiunge la riproduzione del suono rendendo la lezione se possibile anche interattiva.

## Prerequisiti

Comprensione di base di un grafico cartesiano (asse x = tempo, asse y = ampiezza/valore).

Capacità di leggere valori su un asse graduato.

Concetto intuitivo di "segnale che cambia nel tempo" (es. volume della musica, altezza di una collina).

Concetto di approssimazione (arrotondamento a un valore vicino).

### Percorso

Questa attività può essere considerata autoconsistente per introdurre i concetti base, può però far parte di un percorso più ampio sull' introduzione al suono come onda (Scienze/Musica).

Questa unità didattica può definirsi come: "Campionamento e quantizzazione unplugged". Ad essa, si possono collegare in incontri successivi dei passaggi come:

- Introduzione alla rappresentazione binaria dei numeri (collegare i livelli di quantizzazione ai bit)
- Utilizzo di software semplice di editing audio (es. Audacity) per visualizzare forme d'onda reali e gli effetti di cambi di frequenza di campionamento/bit depth (collegamento al concreto)
- Discussione sulla compressione audio come passo successivo.

## Contenuti (spiegati a un informatico)

**Conversione Analogico-Digitale (ADC)**

**Campionamento**: Discretizzazione dell'asse temporale. Acquisizione del valore del segnale a intervalli regolari T (periodo di campionamento). Frequenza di campionamento fs = 1/T. (Si introduce solo l'idea intuitiva che campionare più spesso cattura meglio le variazioni rapide).

**Quantizzazione**: Discretizzazione dell'asse delle ampiezze. Approssimazione del valore campionato al livello più vicino tra un insieme finito di livelli discreti (Quantizzazione scalare uniforme). Il numero di livelli è legato alla risoluzione (bit depth). (Si introduce solo l'idea di "arrotondare" a valori predefiniti).

**Errore di quantizzazione**: Differenza tra l'ampiezza esatta del campione e il valore digitale assegnato dalla quantizzazione. È l'inevitabile scarto dovuto all'approssimazione a livelli finiti.

**Rappresentazione digitale come sequenza di numeri**: Il segnale audio, dopo campionamento e quantizzazione, diventa una successione di valori numerici. Ogni numero codifica l'ampiezza di un campione in un preciso istante.

## Grandi idee

**Rappresentazione dei Dati**: Come l'informazione continua del mondo reale (suono) viene rappresentata in forma discreta (numeri) comprensibile a un computer.

**Astrazione**: Il processo di campionamento e quantizzazione è un'astrazione che semplifica la complessità del segnale reale, perdendo dettagli ma rendendolo manipolabile.

**Algoritmi**: La sequenza di passi (disegna -> misura a intervalli -> arrotonda ai livelli) è un algoritmo per la conversione A/D.

## Traguardi e obiettivi

### Traguardi/obiettivi generali dai documenti ministeriali/proposte

Traguardi/obiettivi generali dai documenti ministeriali/proposte: 

Comprendere il concetto di **campionamento** di un segnale audio.
Intuire il significato di **quantizzazione** e di **perdita di informazione**.
Collegare il mondo fisico (suono) con la sua rappresentazione digitale.
Favorire il pensiero **computazionale** attraverso la rappresentazione di dati continui in forma discreta.
Stimolare l’ **osservazione critica** e il **ragionamento scientifico**.

Obiettivi specifici in forma operativa (Lo studente/la studentessa è in grado di...):

(Ricordare) Elencare i due passaggi principali della digitalizzazione audio (campionamento, quantizzazione).

(Comprendere) Spiegare a parole proprie la differenza tra un'onda disegnata liscia (analogica) e una a gradini (digitale).
(Comprendere) Spiegare perché il campionamento consiste nel misurare il segnale a intervalli regolari.
(Comprendere) Spiegare perché la quantizzazione consiste nell'arrotondare il valore misurato a livelli predefiniti.

(Applicare) Disegnare una semplice curva continua su carta millimetrata per rappresentare un segnale analogico.
(Applicare) Identificare e segnare i punti di campionamento su una curva data, secondo un intervallo specificato.
(Applicare) Approssimare il valore di ciascun campione al livello di quantizzazione più vicino su un grafico.
(Applicare) Ricostruire graficamente (a gradini) il segnale digitale partendo dai punti quantizzati.
(Analizzare) Confrontare il segnale originale e quello digitale ricostruito, identificando le differenze.

(Valutare) Prevedere (intuitivamente) l'effetto sulla fedeltà del segnale digitale cambiando la frequenza di campionamento (intervallo tra i punti).
(Valutare) Prevedere (intuitivamente) l'effetto sulla fedeltà del segnale digitale cambiando il numero di livelli di quantizzazione.

## Metodologie didattiche

**Unplugged Activity**: Attività svolta senza l'uso di computer, utilizzando materiali concreti (carta, matita) per simulare processi computazionali. Permette di focalizzarsi sui concetti senza la barriera tecnologica.

**Apprendimento Attivo / Learning by Doing**: Gli studenti non sono recettori passivi, ma eseguono attivamente i passaggi di campionamento e quantizzazione.

**Visualizzazione**: L'uso della carta millimetrata e del disegno è centrale per rendere visibili concetti astratti.

**Lezione Dialogata**: L'insegnante guida l'attività, ma stimola la discussione, pone domande e incoraggia la riflessione collettiva.

**(Opzionale) Cooperative Learning**: L'attività può essere svolta a coppie per favorire il confronto e l'aiuto reciproco.

## Tempi

**Totale**: Circa 2 ore (es. 2 moduli da 50-60 minuti).

### Fase 1 - Introduzione e l' onda analogica (15-20 min)

**Guida insegnante**: 

**Azione 1**: Iniziare la lezione ponendo una domanda aperta agli studenti:

"Come pensate che la musica che ascoltate arrivi sui vostri smartphone o computer?"

**Scopo**: Raccogliere le loro idee iniziali, stimolare la discussione e creare un collegamento con la loro esperienza quotidiana. Lasciare che emergano diverse ipotesi per poi disegnare su lavagna un' onda sonora illustrando brevemente di cosa si tratta.

**Azione 2**: Chiedere agli studenti di disegnare la propria onda sonora personale, con una frase come:

"Ora disegnate con una matita la vostra onda sonora sulla carta millimetrata. Usate l'asse orizzontale per il tempo e quello verticale per il volume. Disegnate a vostra scelta: una sinusoide, un' onda quadra, una triangolare o a dente di sega."

Nel mentre della richiesta sarebbe bene disegnare gli esempi delle divese onde sonore per agevolare chi ha più difficoltà nel disegno.

**Guida studente**:

Disegnare l' onda sonora secondo le richieste del docente (tipologai di onda, utilizzo di matita).

Si raccomanda una lineea di minimo e una di massimo distanti 12.8 cm (o 25.6), in modo da leggere i millimetri. 

### Fase 2 - Campionamento - Fare le "fotografie" (20-25 min)

**Guida insegnante**:

Spiegare: "Il computer non può 'vedere' tutta la curva contemporaneamente. Deve guardarla un pezzetto alla volta, a intervalli regolari. È come fare delle foto (o misurare l'altezza) dell'onda ogni secondo, o ogni mezzo secondo. Questo si chiama **campionamento**."

Decidere insieme una "frequenza di campionamento" visiva. Suggerimento: "Proviamo a misurare la nostra onda ogni 3 quadretti sull'asse del tempo." (Scegliere un intervallo che generi un numero ragionevole di campioni, es. 8-15 punti).

Dimostrare alla lavagna/LIM: sull'onda disegnata, segnare un punto esattamente sulla curva in corrispondenza di x=0, x=3, x=6, x=9, ecc.

**Guida studente**:

"Prendete la vostra matita (o un colore diverso). Partendo dall'inizio della vostra curva (tempo=0), fate un puntino sulla curva ogni 3 quadretti che avanzate sull'asse del tempo. Continuate finché non finite la parte disegnata della vostra onda."

Girare tra i banchi per verificare che i punti siano sulla curva e a intervalli regolari sull'asse X.

Discussione guidata: "Cosa rappresentano questi punti? (Sono le nostre 'misure' o 'foto' dell'onda in precisi istanti). Cosa succederebbe se facessimo le foto più spesso, ad esempio ogni quadretto? (Avremmo più punti, cattureremmo meglio le curve veloci). E se le facessimo più raramente, ogni 6 quadretti? (Avremmo meno punti, potremmo 'perderci' delle curve veloci tra una foto e l'altra)." Introdurre l'idea intuitiva che più campioni = più fedeltà nel tempo.

### Fase 3 - Quantizzazione - Arrotondare l'altezza (20-25 min)

**Guida insegnante**:

Spiegare: "Ora abbiamo le nostre 'foto' (i campioni). Ma guardate l'altezza (il valore Y) di questi punti: possono capitare ovunque! Il computer, però, preferisce usare solo un numero limitato di 'livelli' di altezza. Dobbiamo prendere l'altezza di ogni punto che abbiamo segnato e 'arrotondarla' al livello permesso più vicino. Questo si chiama Quantizzazione."

Decidere insieme i livelli di quantizzazione. Suggerimento: Sulla carta millimetrata, evidenziare (magari con un tratto leggero di un altro colore o ripassando la linea) le linee orizzontali corrispondenti a valori Y interi (..., -2, -1, 0, 1, 2, 3, ...). Oppure, se la curva è tutta positiva, solo 0, 1, 2, 3... Assegnare un numero (il valore Y) a ciascuna linea evidenziata. Questi sono i nostri "livelli consentiti".

Dimostrare alla lavagna/LIM: Prendere un punto di campionamento. Guardare la sua altezza Y. Trovare la linea orizzontale (livello consentito) più vicina a quel punto. Segnare un nuovo punto (es. una crocetta) che ha la stessa X del campione originale, ma la cui Y è esattamente sul livello consentito più vicino. Ripetere per alcuni campioni.

**Guida studente**:

"Ora, per ogni puntino di campionamento che avete fatto prima, guardate la sua altezza (il suo valore Y). Trovate qual è la linea orizzontale dei 'livelli consentiti' (quelle che abbiamo deciso/evidenziato) più vicina a quel punto. Fate una crocetta (o usate un altro colore) che stia sulla stessa linea verticale (stessa X) del puntino, ma esattamente sulla linea orizzontale consentita più vicina."

Girare tra i banchi aiutando a trovare il livello più vicino. Questo è il passaggio concettualmente più delicato.

**Istruzione Aggiuntiva**: "Ora, per ogni crocetta che avete fatto, scrivete sotto (o a fianco) il numero del livello su cui si trova. Fatelo in ordine, da sinistra a destra. Questa sequenza di numeri è il nostro 'segnale digitale'!"

**Discussione Guidata**: "L'altezza delle crocette è esattamente uguale a quella dei puntini originali? (No, è approssimata). Cosa succederebbe se avessimo meno livelli consentiti, ad esempio solo le linee 0, 2, 4...? (L'approssimazione sarebbe più 'grossolana', perderemmo più dettagli sull'altezza). E se avessimo più livelli, ad esempio anche le linee intermedie a metà quadretto? (L'approssimazione sarebbe più precisa)." Introdurre l'idea intuitiva che più livelli = più fedeltà nell'ampiezza.


### Fase 4 - Ricostruzione e confronto (15-20 min)

**Guida insegnante**:

Spiegare: "Abbiamo la nostra sequenza di numeri, che rappresenta il suono digitalizzato. Come possiamo visualizzare questa versione digitale?"

Dimostrare alla lavagna/LIM: Collegare le crocette (i punti quantizzati) usando solo segmenti orizzontali e verticali. Da una crocetta, tracciare un segmento orizzontale fino alla X della crocetta successiva, poi un segmento verticale per raggiungerla. Si formerà un grafico "a gradini" (staircase).

**Guida studente**:

"Usando una matita colorata (diversa da quella dell'onda originale), collegate le crocette che avete segnato. Partite dalla prima crocetta a sinistra: disegnate una linea orizzontale fino a raggiungere la verticale della seconda crocetta, poi salite o scendete in verticale per collegarvi alla seconda crocetta. 

Ripetete il processo per collegare tutte le crocette. Otterrete una forma a gradini."

## Fase 5: Variare i parametri e conclusioni (20-30 min)

### Guida insegnante

Introdurre l'idea del trade-off. 

"Abbiamo visto che per avere un segnale digitale più fedele all'originale, potremmo campionare più spesso e usare più livelli di quantizzazione. Ma cosa comporterebbe questo?"

Attività di riflessione (anche solo discussa o con un secondo foglio se c'è tempo):

"Immaginate di rifare tutto campionando ogni quadretto invece che ogni 3. Avremmo più o meno punti? (Più punti). Scriveremmo più o meno numeri? (Più numeri). Il disegno a gradini sarebbe più o meno simile all'originale? (Più simile)." -> Alta frequenza di campionamento = Più dati, Maggiore fedeltà (nel tempo).

"Immaginate di rifare tutto usando il doppio dei livelli di quantizzazione (anche le linee a metà quadretto). L'approssimazione dell'altezza sarebbe migliore o peggiore? (Migliore). I numeri che scriviamo sarebbero più 'precisi', magari avremmo bisogno di più cifre o simboli per distinguerli tutti (collegamento intuitivo ai bit). Il disegno a gradini sarebbe più o meno simile all'originale? (Più simile)." -> Più livelli di quantizzazione = Più dati (per campione), Maggiore fedeltà (nell'ampiezza).

"E se campionassimo più raramente (es. ogni 6 quadretti) e usassimo pochissimi livelli (es. solo 3 livelli: 'basso', 'medio', 'alto')? (Avremmo pochi numeri, il segnale sarebbe molto diverso dall'originale, perderemmo molti dettagli)." -> Bassa qualità = Meno dati, Minore fedeltà.
Collegamento al Reale: Spiegare che questo è quello che succede nella realtà:

CD Audio: Alta frequenza di campionamento (44100 volte al secondo!) e molti livelli (65536 livelli - 16 bit) -> Alta fedeltà, file grandi.

MP3/Streaming bassa qualità: Parametri ridotti (o tecniche più complesse di compressione) -> Fedeltà minore, file piccoli.

Telefonate: Qualità sufficiente per capire la voce, ma non ottimale per la musica.


### Discussione guidata

Facilitare il confronto: 

"Dove vedete le differenze maggiori? La forma a gradini segue l'originale? Esattamente? 

Cosa è andato 'perso' nel processo? (La 'morbidezza', i valori intermedi). 

Questa forma a gradini rappresenta il suono come lo sentirebbe il computer, basandosi solo sui numeri che abbiamo ottenuto."




## Spazi

Aula scolastica standard con banchi adatti per disegnare.

Lavagna o LIM per le spiegazioni e dimostrazioni dell'insegnante.

## Materiali e Strumenti

Fogli di carta millimetrata (almeno 2-3 per studente/coppia).

Matite con punta media (HB o simile).

Gomme per cancellare.

Matite colorate o pennarelli a punta fine (almeno 2 colori diversi per studente/coppia, es. nero e rosso).

Righello (opzionale, può aiutare a tracciare i livelli di quantizzazione).

Lavagna/LIM e pennarelli/pennino.

# Conclusione

Riepilogare i termini chiave (Analogico, Digitale, Campionamento, Quantizzazione) e il concetto principale: la digitalizzazione è un'approssimazione del mondo reale fatta misurando a intervalli (campionamento) e arrotondando i valori (quantizzazione), con un compromesso tra fedeltà e quantità di dati generati.

Valutazione Formativa e Continuativa (Suggerimenti per l'insegnante):

Osservazione durante le attività: Verificare se gli studenti seguono le istruzioni, se posizionano correttamente i punti di campionamento e quantizzazione. Notare chi ha difficoltà e fornire supporto individuale.

Domande durante la discussione: Porre domande mirate per verificare la comprensione ("Perché stiamo mettendo i punti solo ogni 3 quadretti?", "Perché la crocetta non è esattamente sopra il puntino originale?", "Cosa cambierebbe se...").

Analisi dei grafici prodotti: Raccogliere (anche temporaneamente) i fogli per osservare il risultato finale. Il confronto tra l'onda originale e quella a gradini è un buon indicatore della comprensione del processo di approssimazione.

Al termine dell’attività, gli studenti producono:

- Una rappresentazione grafica del segnale campionato su carta millimetrata;

- Una tabella con i valori numerici ottenuti dalla quantizzazione;

- Una breve riflessione scritta o orale (individuale o di gruppo) su cosa hanno scoperto e imparato.

Ciò che si valuta sono: accuratezza, coerenza con la traccia, uso corretto dei termini.


Il materiale principale sono i fogli di carta millimetrata e le istruzioni verbali/dimostrazioni dell'insegnante. Non è previsto materiale cartaceo aggiuntivo per mantenere la natura fluida e adattabile dell'attività unplugged, ma si potrebbe fornire un foglio riassuntivo alla fine con i termini chiave e una definizione semplice.

# Bibliografia

Citare le fonti utilizzate (si consiglia ad esempio bibtex o biblatex).
Scegliere lo stile preferito, e mantenerlo coerente ([esempio](https://www.acm.org/publications/authors/reference-formatting))

# Licenza del documento

CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/deed.it
