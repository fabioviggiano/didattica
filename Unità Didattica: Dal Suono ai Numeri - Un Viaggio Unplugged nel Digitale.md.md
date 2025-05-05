---
title: Titolo Materiale Didattico
author: Fabio Viggiano
date: 12/04/25
---

Esame di Didattica dell'Informatica, A.A. 2024/2025

# Inquadramento del lavoro

## Livello di scuola, classe/i, indirizzo

Livello di scuola, classe/i, indirizzo: Scuola Secondaria di I grado (Scuole Medie), classi prime o seconde. Adattabile anche per le terze.
A chi è rivolta questa attività? Studenti e studentesse di età compresa tra 11 e 13/14 anni.
In quale specifica disciplina scolastica si colloca l'attività?
Disciplina prevalente: Informatica (secondo la Proposta CINI - Area: Rappresentazione dell'Informazione).
Discipline coinvolte: Tecnologia (processi di trasformazione), Matematica (grafici cartesiani, approssimazione), Scienze (onde sonore), Musica (natura del suono).
Può essere adattata/rivolta a studenti di diverse età e indirizzi? Sì.
Scuola Primaria (classi 4-5): Semplificando ulteriormente la terminologia, usando griglie più grandi e meno livelli di quantizzazione, concentrandosi sull'idea di "fare foto" (campionare) e "arrotondare" (quantizzare) un disegno.
Scuola Secondaria di II grado (primo biennio): Introducendo concetti più formali come frequenza di campionamento (Hz), bit depth, teorema di Nyquist (in modo intuitivo), e discutendo maggiormente il trade-off qualità/dimensione file.


## Motivazione e Finalità

Di che attività si tratta: Un'attività pratica e manuale (unplugged) per comprendere i concetti fondamentali della digitalizzazione del suono: campionamento e quantizzazione, usando carta millimetrata e matite.
Perché è importante svolgere questa attività nella scuola? È fondamentale per sviluppare la consapevolezza di come i segnali del mondo reale (analogici) vengono trasformati in dati digitali manipolabili dai computer, alla base di gran parte della tecnologia multimediale che gli studenti usano quotidianamente (musica, video, chiamate). Promuove il pensiero computazionale attraverso l'astrazione e la scomposizione del problema.

## Innovatività

Perché questa proposta è innovativa? Sebbene le attività unplugged per l'informatica siano diffuse (es. CS Unplugged), questa proposta si focalizza specificamente sulla visualizzazione manuale e combinata del campionamento e della quantizzazione su carta millimetrata come processo sequenziale applicato a un segnale disegnato dagli studenti stessi. Rispetto a simulazioni software, l'approccio manuale rinforza la comprensione kinestetica dei passaggi e dell'approssimazione introdotta.
Cosa è già presente e in cosa si differenzia/migliora? Esistono risorse online (es. simulatori interattivi come quello di The Pudding "How Music Taste Evolved" o spiegazioni video) e attività unplugged generiche sulla rappresentazione binaria. CS Unplugged ha attività sulla rappresentazione delle immagini, ma meno focalizzate sul processo A/D audio in questo modo specifico. Questa unità:
Mantiene: L'approccio unplugged e l'uso di metafore concrete.
Differenzia/Migliora: Integra campionamento e quantizzazione in un unico flusso di lavoro manuale, partendo da un "segnale" creato dallo studente, rendendo il processo più personale e tangibile. Enfatizza la visualizzazione della perdita di informazione confrontando il disegno originale con quello "digitalizzato".

## Prerequisiti

Comprensione di base di un grafico cartesiano (asse x = tempo, asse y = ampiezza/valore).
Capacità di leggere valori su un asse graduato.
Concetto intuitivo di "segnale che cambia nel tempo" (es. volume della musica, altezza di una collina).
Concetto di approssimazione (arrotondamento a un valore vicino).

### Percorso

Questa attività può essere considerata autoconsistente per introdurre i concetti base. Può far parte di un percorso più ampio:
Introduzione al suono come onda (Scienze/Musica).
Questa Unità Didattica: Campionamento e Quantizzazione Unplugged.
(Opzionale) Introduzione alla rappresentazione binaria dei numeri (collegare i livelli di quantizzazione ai bit).
(Opzionale) Utilizzo di software semplice di editing audio (es. Audacity) per visualizzare forme d'onda reali e gli effetti di cambi di frequenza di campionamento/bit depth (collegamento al concreto).
(Opzionale) Discussione sulla compressione audio (MP3, etc.) come passo successivo.

## Contenuti (spiegati a un informatico)

Conversione Analogico-Digitale (ADC).
Campionamento: Discretizzazione dell'asse temporale. Acquisizione del valore del segnale a intervalli regolari T (periodo di campionamento). Frequenza di campionamento fs = 1/T. (Si introduce solo l'idea intuitiva che campionare più spesso cattura meglio le variazioni rapide).
Quantizzazione: Discretizzazione dell'asse delle ampiezze. Approssimazione del valore campionato al livello più vicino tra un insieme finito di livelli discreti (Quantizzazione scalare uniforme). Il numero di livelli è legato alla risoluzione (bit depth). (Si introduce solo l'idea di "arrotondare" a valori predefiniti).
Errore di quantizzazione.
Rappresentazione digitale come sequenza di numeri.

## Grandi idee

Rappresentazione dei Dati: Come l'informazione continua del mondo reale (suono) viene rappresentata in forma discreta (numeri) comprensibile a un computer.
Astrazione: Il processo di campionamento e quantizzazione è un'astrazione che semplifica la complessità del segnale reale, perdendo dettagli ma rendendolo manipolabile.
Algoritmi: La sequenza di passi (disegna -> misura a intervalli -> arrotonda ai livelli) è un algoritmo per la conversione A/D.


## Traguardi e Obiettivi
Nelle varie sottosezioni, vanno elencati traguardi e obiettivi di apprendimento che si vuole raggiungere con le attività proposte

### Traguardi/obiettivi generali dai documenti ministeriali/proposte

Traguardi/obiettivi generali dai documenti ministeriali/proposte:
(Indicazioni Nazionali Primo Ciclo - Tecnologia): "Utilizzare strumenti informatici e di comunicazione [...] per ricercare, progettare [...]". "Riconoscere nell'ambiente che lo circonda [...] i processi di trasformazione di risorse e di energia [...]". (Qui la trasformazione è del segnale).
(Proposta CINI - Scuola Secondaria I Grado):
Area Dati e Informazione, Rappresentazione dell'informazione: D-RI.1: Comprendere che le informazioni possono essere rappresentate in modi diversi (analogico vs digitale). D-RI.2: Spiegare come diversi tipi di dati (numeri, testi, immagini, suoni) sono rappresentati in formato digitale (focus su suoni). D-RI.3: Comprendere il concetto di digitalizzazione e i suoi effetti (approssimazione, perdita di informazione).
Traguardi/obiettivi generali (propri):
Comprendere la differenza fondamentale tra segnale analogico e digitale.
Afferrare il ruolo del campionamento e della quantizzazione nel processo di digitalizzazione.
Sviluppare un'intuizione sulla relazione tra parametri di digitalizzazione (frequenza campionamento, livelli quantizzazione) e fedeltà/quantità di dati.
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

Unplugged Activity: Attività svolta senza l'uso di computer, utilizzando materiali concreti (carta, matita) per simulare processi computazionali. Permette di focalizzarsi sui concetti senza la barriera tecnologica.
Apprendimento Attivo / Learning by Doing: Gli studenti non sono recettori passivi, ma eseguono attivamente i passaggi di campionamento e quantizzazione.
Visualizzazione: L'uso della carta millimetrata e del disegno è centrale per rendere visibili concetti astratti.
Lezione Dialogata: L'insegnante guida l'attività, ma stimola la discussione, pone domande e incoraggia la riflessione collettiva.
(Opzionale) Cooperative Learning: L'attività può essere svolta a coppie per favorire il confronto e l'aiuto reciproco.

## Tempi

Totale: Circa 2 ore (es. 2 moduli da 50-60 minuti).
Introduzione e disegno onda analogica: 15-20 min.
Attività di Campionamento: 20-25 min.
Attività di Quantizzazione: 20-25 min.
Ricostruzione e Confronto: 15-20 min.
Discussione su Variazione Parametri e Conclusioni: 20-30 min.

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

# Sviluppo dei contenuti

(Guida per gli Insegnanti inframezzata alle fasi)
Fase 1: Introduzione e L'Onda Analogica (15-20 min)
Guida Insegnante:
Iniziare chiedendo agli studenti come pensano che la musica arrivi ai loro telefoni o computer. Introdurre l'idea di suono come qualcosa di "continuo" nel mondo reale (un'onda) che deve essere trasformato in "numeri" per il computer (digitale).
Disegnare alla lavagna/LIM un esempio semplice di onda: un asse X (tempo) e un asse Y (volume/ampiezza). Tracciare una curva morbida e continua.
Enfatizzare: "Questa linea è continua. Significa che per ogni istante di tempo, anche piccolissimo, c'è un valore preciso di volume, e il volume può cambiare in modo graduale assumendo tutti i valori intermedi." Chiamarla "Onda Analogica".
Distribuire carta millimetrata e matite.
Istruzione per Studenti: "Ora disegnate la vostra onda sonora personale sulla carta millimetrata. Usate l'asse orizzontale per il tempo e quello verticale per il volume. Fate una curva semplice, che sale e scende, che occupi una buona parte del foglio in larghezza. Usate la matita così potete correggere."
Girare tra i banchi per assicurarsi che tutti abbiano disegnato una curva adatta (non troppo spigolosa, né troppo piatta).
Fase 2: Campionamento - Fare le "Fotografie" (20-25 min)
Guida Insegnante:
Spiegare: "Il computer non può 'vedere' tutta la curva contemporaneamente. Deve guardarla un pezzetto alla volta, a intervalli regolari. È come fare delle foto (o misurare l'altezza) dell'onda ogni secondo, o ogni mezzo secondo. Questo si chiama Campionamento."
Decidere insieme una "frequenza di campionamento" visiva. Suggerimento: "Proviamo a misurare la nostra onda ogni 3 quadretti sull'asse del tempo." (Scegliere un intervallo che generi un numero ragionevole di campioni, es. 8-15 punti).
Dimostrare alla lavagna/LIM: sull'onda disegnata, segnare un punto esattamente sulla curva in corrispondenza di x=0, x=3, x=6, x=9, ecc.
Istruzione per Studenti: "Prendete la vostra matita (o un colore diverso). Partendo dall'inizio della vostra curva (tempo=0), fate un puntino sulla curva ogni 3 quadretti che avanzate sull'asse del tempo. Continuate finché non finite la parte disegnata della vostra onda."
Girare tra i banchi per verificare che i punti siano sulla curva e a intervalli regolari sull'asse X.
Discussione Guidata: "Cosa rappresentano questi punti? (Sono le nostre 'misure' o 'foto' dell'onda in precisi istanti). Cosa succederebbe se facessimo le foto più spesso, ad esempio ogni quadretto? (Avremmo più punti, cattureremmo meglio le curve veloci). E se le facessimo più raramente, ogni 6 quadretti? (Avremmo meno punti, potremmo 'perderci' delle curve veloci tra una foto e l'altra)." Introdurre l'idea intuitiva che più campioni = più fedeltà nel tempo.
Fase 3: Quantizzazione - Arrotondare l'Altezza (20-25 min)
Guida Insegnante:
Spiegare: "Ora abbiamo le nostre 'foto' (i campioni). Ma guardate l'altezza (il valore Y) di questi punti: possono capitare ovunque! Il computer, però, preferisce usare solo un numero limitato di 'livelli' di altezza. Dobbiamo prendere l'altezza di ogni punto che abbiamo segnato e 'arrotondarla' al livello permesso più vicino. Questo si chiama Quantizzazione."
Decidere insieme i livelli di quantizzazione. Suggerimento: Sulla carta millimetrata, evidenziare (magari con un tratto leggero di un altro colore o ripassando la linea) le linee orizzontali corrispondenti a valori Y interi (..., -2, -1, 0, 1, 2, 3, ...). Oppure, se la curva è tutta positiva, solo 0, 1, 2, 3... Assegnare un numero (il valore Y) a ciascuna linea evidenziata. Questi sono i nostri "livelli consentiti".
Dimostrare alla lavagna/LIM: Prendere un punto di campionamento. Guardare la sua altezza Y. Trovare la linea orizzontale (livello consentito) più vicina a quel punto. Segnare un nuovo punto (es. una crocetta) che ha la stessa X del campione originale, ma la cui Y è esattamente sul livello consentito più vicino. Ripetere per alcuni campioni.
Istruzione per Studenti: "Ora, per ogni puntino di campionamento che avete fatto prima, guardate la sua altezza (il suo valore Y). Trovate qual è la linea orizzontale dei 'livelli consentiti' (quelle che abbiamo deciso/evidenziato) più vicina a quel punto. Fate una crocetta (o usate un altro colore) che stia sulla stessa linea verticale (stessa X) del puntino, ma esattamente sulla linea orizzontale consentita più vicina."
Girare tra i banchi aiutando a trovare il livello più vicino. Questo è il passaggio concettualmente più delicato.
Istruzione Aggiuntiva: "Ora, per ogni crocetta che avete fatto, scrivete sotto (o a fianco) il numero del livello su cui si trova. Fatelo in ordine, da sinistra a destra. Questa sequenza di numeri è il nostro 'segnale digitale'!"
Discussione Guidata: "L'altezza delle crocette è esattamente uguale a quella dei puntini originali? (No, è approssimata). Cosa succederebbe se avessimo meno livelli consentiti, ad esempio solo le linee 0, 2, 4...? (L'approssimazione sarebbe più 'grossolana', perderemmo più dettagli sull'altezza). E se avessimo più livelli, ad esempio anche le linee intermedie a metà quadretto? (L'approssimazione sarebbe più precisa)." Introdurre l'idea intuitiva che più livelli = più fedeltà nell'ampiezza.
Fase 4: Ricostruzione e Confronto (15-20 min)
Guida Insegnante:
Spiegare: "Abbiamo la nostra sequenza di numeri, che rappresenta il suono digitalizzato. Come possiamo visualizzare questa versione digitale?"
Dimostrare alla lavagna/LIM: Collegare le crocette (i punti quantizzati) usando solo segmenti orizzontali e verticali. Da una crocetta, tracciare un segmento orizzontale fino alla X della crocetta successiva, poi un segmento verticale per raggiungerla. Si formerà un grafico "a gradini" (staircase).
Istruzione per Studenti: "Usando una matita colorata (diversa da quella dell'onda originale), collegate le crocette che avete segnato. Partite dalla prima crocetta a sinistra: disegnate una linea orizzontale fino a raggiungere la verticale della seconda crocetta, poi salite o scendete in verticale per collegarvi alla seconda crocetta. Ripetete il processo per collegare tutte le crocette. Otterrete una forma a gradini."
Istruzione per Studenti: "Ora confrontate la vostra onda originale (quella liscia disegnata all'inizio) con questa nuova forma a gradini. Sono uguali?"
Discussione Guidata: Facilitare il confronto: "Dove vedete le differenze maggiori? La forma a gradini segue l'originale? Esattamente? Cosa è andato 'perso' nel processo? (La 'morbidezza', i valori intermedi). Questa forma a gradini rappresenta il suono come lo sentirebbe il computer, basandosi solo sui numeri che abbiamo ottenuto."
Fase 5: Variare i Parametri e Conclusioni (20-30 min)
Guida Insegnante:
Introdurre l'idea del trade-off. "Abbiamo visto che per avere un segnale digitale più fedele all'originale, potremmo campionare più spesso e usare più livelli di quantizzazione. Ma cosa comporterebbe questo?"
Attività di Riflessione (anche solo discussa o con un secondo foglio se c'è tempo):
"Immaginate di rifare tutto campionando ogni quadretto invece che ogni 3. Avremmo più o meno punti? (Più punti). Scriveremmo più o meno numeri? (Più numeri). Il disegno a gradini sarebbe più o meno simile all'originale? (Più simile)." -> Alta frequenza di campionamento = Più dati, Maggiore fedeltà (nel tempo).
"Immaginate di rifare tutto usando il doppio dei livelli di quantizzazione (anche le linee a metà quadretto). L'approssimazione dell'altezza sarebbe migliore o peggiore? (Migliore). I numeri che scriviamo sarebbero più 'precisi', magari avremmo bisogno di più cifre o simboli per distinguerli tutti (collegamento intuitivo ai bit). Il disegno a gradini sarebbe più o meno simile all'originale? (Più simile)." -> Più livelli di quantizzazione = Più dati (per campione), Maggiore fedeltà (nell'ampiezza).
"E se campionassimo più raramente (es. ogni 6 quadretti) e usassimo pochissimi livelli (es. solo 3 livelli: 'basso', 'medio', 'alto')? (Avremmo pochi numeri, il segnale sarebbe molto diverso dall'originale, perderemmo molti dettagli)." -> Bassa qualità = Meno dati, Minore fedeltà.
Collegamento al Reale: Spiegare che questo è quello che succede nella realtà:
CD Audio: Alta frequenza di campionamento (44100 volte al secondo!) e molti livelli (65536 livelli - 16 bit) -> Alta fedeltà, file grandi.
MP3/Streaming bassa qualità: Parametri ridotti (o tecniche più complesse di compressione) -> Fedeltà minore, file piccoli.
Telefonate: Qualità sufficiente per capire la voce, ma non ottimale per la musica.
Conclusione: Riepilogare i termini chiave (Analogico, Digitale, Campionamento, Quantizzazione) e il concetto principale: la digitalizzazione è un'approssimazione del mondo reale fatta misurando a intervalli (campionamento) e arrotondando i valori (quantizzazione), con un compromesso tra fedeltà e quantità di dati generati.
Valutazione Formativa e Continuativa (Suggerimenti per l'insegnante):
Osservazione durante le attività: Verificare se gli studenti seguono le istruzioni, se posizionano correttamente i punti di campionamento e quantizzazione. Notare chi ha difficoltà e fornire supporto individuale.
Domande durante la discussione: Porre domande mirate per verificare la comprensione ("Perché stiamo mettendo i punti solo ogni 3 quadretti?", "Perché la crocetta non è esattamente sopra il puntino originale?", "Cosa cambierebbe se...").
Analisi dei grafici prodotti: Raccogliere (anche temporaneamente) i fogli per osservare il risultato finale. Il confronto tra l'onda originale e quella a gradini è un buon indicatore della comprensione del processo di approssimazione.
(Opzionale) Breve quiz/domanda aperta alla fine: Chiedere di spiegare a parole proprie uno dei concetti chiave o di disegnare un esempio semplice.
(Materiale per Studenti): Il materiale principale sono i fogli di carta millimetrata e le istruzioni verbali/dimostrazioni dell'insegnante. Non è previsto materiale cartaceo aggiuntivo per mantenere la natura fluida e adattabile dell'attività unplugged, ma si potrebbe fornire un foglio riassuntivo alla fine con i termini chiave e una definizione semplice.

# Bibliografia

Citare le fonti utilizzate (si consiglia ad esempio bibtex o biblatex).
Scegliere lo stile preferito, e mantenerlo coerente ([esempio](https://www.acm.org/publications/authors/reference-formatting))

# Licenza del documento

CC BY-SA 4.0
