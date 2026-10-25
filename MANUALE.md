# S33 - Loopscape: manuale d'uso

Questa guida spiega come usare Loopscape, dai concetti di base alla gestione delle scene per un'esibizione dal vivo. Per installazione e pubblicazione dell'app vedi il [README](README.md).

## Indice

1. [Concetti di base](#1-concetti-di-base)
2. [Prima sessione](#2-prima-sessione)
3. [Interfaccia](#3-interfaccia)
4. [Disegnare](#4-disegnare)
5. [Barra del loop](#5-barra-del-loop)
6. [Striscia delle percussioni](#6-striscia-delle-percussioni)
7. [Ritmo a step](#7-ritmo-a-step)
8. [Armonia](#8-armonia)
9. [Tempo, durata e BPM](#9-tempo-durata-e-bpm)
10. [Mixer e suono](#10-mixer-e-suono)
11. [Scene](#11-scene)
12. [Salvataggio dei dati](#12-salvataggio-dei-dati)
13. [Scorciatoie da tastiera](#13-scorciatoie-da-tastiera)
14. [Idee e ricette](#14-idee-e-ricette)
15. [Risoluzione dei problemi](#15-risoluzione-dei-problemi)
16. [Riferimento delle impostazioni](#16-riferimento-delle-impostazioni)

---

## 1. Concetti di base

Loopscape è una lavagna bianca che suona. Si disegna con il dito o con l'Apple Pencil, poi una linea verticale, la **playhead**, scorre da sinistra a destra e, quando tocca un disegno, produce un suono. Arrivata a destra ricomincia da sinistra, finché non premi Stop.

- **Asse orizzontale = tempo.** Ciò che disegni a sinistra suona prima di ciò che disegni a destra.
- **Asse verticale = altezza della nota.** In alto le note sono acute, in basso gravi. Nell'area melodica l'estensione è di circa quattro ottave, da Do2 a Do6.
- **Colore = strumento.** Blu drone, viola arpeggio, ambra campana, verde pad.
- **Spessore = intensità.** Un tratto spesso suona più forte e, a seconda dello strumento, più a lungo.
- **Giro (o loop):** un passaggio completo della playhead. La sua durata si imposta in secondi oppure si ricava da un BPM (capitolo 9).
- **Quarti e accordi.** La lavagna è divisa in quattro quarti uguali, e ognuno ha il suo accordo, scritto in alto. Una nota disegnata in un quarto si aggancia all'accordo e alla scala di quel quarto. Per questo qualsiasi scarabocchio resta intonato.
- **Tonalità e scala.** Sono scelte a caso all'avvio o impostate da te, e compaiono sotto il titolo (ad esempio «Re dorico»).
- **Striscia ritmica.** Il 30% inferiore della lavagna è riservato alle percussioni.

```
┌──────────────────────────────────────────────────────┐
│ ▮                  barra del loop                  ▮ │
│ accordo 1     accordo 2     accordo 3     accordo 4  │
│                                                      │
│   area melodica: altezza = nota                      │
│   droni, arpeggi, campane, pad                       │
│                                                      │
├──────────────────────────────────────────────────────┤
│ Bongo alto                                           │
│ Bongo basso          striscia delle percussioni      │
│ Legno                                                │
│ Marimba                                              │
│ Vetro                                                │
└──────────────────────────────────────────────────────┘
        ◄── la playhead scorre da sinistra a destra ──►
```

## 2. Prima sessione

1. Tocca **Play**. Il suono parte solo dopo questo tocco: su iPhone e iPad è una regola del sistema.
2. Con **Drone** (blu) selezionato, disegna una linea orizzontale nella parte bassa. Quando la playhead la attraversa senti una nota tenuta.
3. Scegli **Campana** (ambra) e disegna una curva nella parte alta. Ogni tratto di linea produce una nota.
4. Tocca alcuni punti nella **striscia viola** in basso: sono colpi di percussione che si ripetono a ogni giro.
5. Apri **Ritmo**, attiva l'interruttore **Attivo** e tocca qualche cella della griglia.
6. Apri **Impostazioni** e prova a muovere BPM, Durata e Tonalità.
7. Se ti piace il risultato, apri **Scene** e tocca **+ Nuova** per salvarlo.

## 3. Interfaccia

**Barra in alto**

| Controllo | Funzione |
|---|---|
| **Play / Stop** | Avvia e ferma la riproduzione. Stop riporta la playhead all'inizio e lascia sfumare i suoni in corso. |
| **Annulla** | Toglie l'ultimo tratto disegnato. |
| **Cancella** | Svuota la lavagna. Il primo tocco chiede conferma (il pulsante diventa rosso per qualche secondo), il secondo cancella. |
| **Ritmo** | Apre il pannello dello step sequencer. Si illumina quando il ritmo è attivo e lampeggia a ogni colpo. |
| **Scene** | Apre l'archivio delle scene. |
| **Titolo e tonalità** | «S33 - Loopscape» e, sotto, tonalità e scala correnti. |
| **Impostazioni** | L'icona con i cursori, a destra: apre il foglio delle impostazioni. |

**Barra in basso**

| Controllo | Funzione |
|---|---|
| **Drone, Arpeggio, Campana, Pad** | Scelgono lo strumento con cui disegni. Quello attivo ha il bordo evidenziato. |
| **Gomma** | Cancella ciò che tocchi. |
| **Magnete** | Attiva o disattiva la griglia magnetica. |
| **Cursore dello spessore** | Imposta spessore e intensità di ciò che disegni; il pallino a sinistra ne mostra la misura. |

Sugli schermi stretti (iPhone in verticale) i nomi dei pulsanti in alto scompaiono e restano le icone, e il titolo si sposta su una riga a parte.

**Segnali visivi.** Quando una nota suona, dal punto del disegno parte un'onda circolare del colore dello strumento. Il quarto che la playhead sta attraversando è leggermente evidenziato.

L'interfaccia segue il tema chiaro o scuro del sistema; la lavagna resta sempre bianca.

## 4. Disegnare

### Gli strumenti

| Strumento | Colore | Come suona | Effetto dello spessore |
|---|---|---|---|
| **Drone** | Blu | Una nota tenuta e continua, che dura finché la playhead attraversa la linea. Cambiando altezza scivola da una nota all'altra. Si appoggia sempre su fondamentale e quinta dell'accordo. Il timbro è caldo, con un filtro che respira lentamente. | Più spesso = più forte. |
| **Arpeggio** | Viola | Le note dell'accordo suonate in sequenza, salendo e scendendo attorno all'altezza della linea, per tutto il tempo in cui la playhead la attraversa. | Più spesso = più lento, più forte e con code più lunghe. |
| **Campana** | Ambra | Una nota a intervalli regolari lungo il tratto, agganciata alla scala. Timbro metallico, con una coda lunga. | Più spesso = più forte e più lunga. |
| **Pad** | Verde | Note lunghe e morbide dell'accordo, a intervalli più radi, con attacco lento. | Più spesso = più forte e più lungo. |

Campana e pad suonano una nota ogni tratto di lunghezza: più lungo è il tratto, più note produce, a prescindere dalla velocità con cui lo disegni. Drone e arpeggio invece suonano solo mentre la playhead si trova sopra l'estensione orizzontale del tratto: una linea lunga dà un suono lungo, una breve un suono breve.

Se una linea attraversa la playhead in più punti nello stesso istante (per esempio una curva a onda), il drone segue il punto più basso e l'arpeggio il più alto.

### Spessore e Apple Pencil

Il cursore in basso va da sottile a spesso. Con l'Apple Pencil la pressione modula lo spessore, da circa metà fino a una volta e mezza il valore impostato: puoi quindi dare dinamica alla stessa linea.

Quando usi la penna, i tocchi delle dita nel secondo e mezzo successivo vengono ignorati, così il palmo appoggiato non lascia segni.

### Gomma, Annulla e Cancella

- **Gomma:** tocca o trascina. Cancella i tratti sotto il cerchietto; nella striscia delle percussioni rimuove i singoli colpi.
- **Annulla:** rimuove l'ultimo tratto, anche se è una serie di colpi disegnata con un solo gesto.
- **Cancella:** svuota tutto, con conferma.

### Magnete

Con il pulsante **Magnete** acceso, ogni punto del tratto si aggancia all'incrocio più vicino di una griglia: orizzontalmente alle colonne, verticalmente alle note della scala corrente. Il risultato sono linee precise, a scalini o diagonali pulite, di lunghezza a piacere.

- La densità si sceglie in Impostazioni → **Griglia magnetica**: 8, 16, 32, 64 o 128 colonne (le ultime due per la massima precisione).
- Vale solo nell'area melodica; la striscia delle percussioni ha una griglia propria (capitolo 6).
- Con il magnete acceso anche le maniglie della barra del loop si agganciano a questa griglia.
- Per attivare le linee delle note sullo sfondo, usa «Mostra la griglia delle note» nelle Impostazioni.

## 5. Barra del loop

La fascia sottile in cima alla lavagna contiene due **maniglie blu**. Trascinale per far girare la playhead solo su una parte della lavagna.

- **Maniglia sinistra o destra:** trascinala per spostare l'inizio o la fine del giro.
- **Zona blu in mezzo:** trascinala per spostare la regione senza cambiarne la larghezza.
- **Doppio tocco sulla barra:** torna all'intera lavagna. Lo stesso fa il pulsante «Loop sull'intera lavagna» nelle Impostazioni.
- **Aggancio:** le maniglie si agganciano a sedicesimi di lavagna (oppure alla densità del magnete, se acceso). La regione non può essere più stretta di un passo.
- **Fuori regione:** la lavagna si scurisce leggermente. I tratti fuori regione restano muti, ma puoi continuare a disegnare lì e includerli dopo.

Cosa succede al suono:

- **Velocità costante.** La playhead non cambia velocità: una regione più corta dura proporzionalmente meno. Con una durata di 45 secondi, metà lavagna dura 22,5 secondi. La durata della regione appare nelle Impostazioni, nella riga «Regione di loop».
- **Gli accordi restano legati ai quarti.** Se selezioni il secondo e il terzo quarto, il loop suona solo quei due accordi. È un modo efficace per costruire una progressione più breve.
- Se sposti le maniglie mentre suona e la playhead finisce fuori regione, salta all'inizio della regione. I droni e le note tenute a cavallo del bordo si chiudono con il loro rilascio morbido.
- **Stop** riporta la playhead all'inizio della regione.

La fascia della barra occupa circa 34 pixel in alto: in quel punto non si disegna.

## 6. Striscia delle percussioni

Il 30% inferiore della lavagna, in viola, è diviso in cinque corsie, ciascuna con il suo strumento:

| Corsia | Suono |
|---|---|
| **Bongo alto** | Colpo di pelle breve e leggero, accordato sull'accordo corrente. |
| **Bongo basso** | Più grave e rotondo, accordato più in basso. |
| **Legno** | Colpo asciutto e corto, con un piccolo click. |
| **Marimba** | Nota morbida: la sua altezza cambia con la posizione orizzontale, scorrendo tra le note dell'accordo. |
| **Vetro** | Timbro etereo e cristallino, nel registro alto, con la stessa logica della marimba. |

**Come si disegna.** Il tratto è un ritmo se parte dentro la striscia. Un tocco è un colpo singolo; trascinando in orizzontale si ottiene una serie regolare; un tratto che attraversa più corsie produce colpi in corsie diverse. Il colore in questa zona non cambia il suono (lo decide la corsia) e serve solo per l'aspetto.

**Intensità.** Lo spessore (o la pressione della penna) decide la forza di ogni colpo.

**Griglia ritmica.** In Impostazioni → *Griglia ritmica (striscia in basso)* scegli quanti passi per giro dividono la striscia:

- **32, 64 o 128:** ogni colpo si aggancia al centro della colonna più vicina. Più passi significano più precisione e colpi più ravvicinati (il predefinito è 64).
- **Libera:** nessun aggancio, i colpi cadono dove li metti.

**Sono colpi fissi.** A ogni giro la striscia ripete gli stessi colpi, senza probabilità né casualità, mentre la playhead li incontra. L'accordo è quello del quarto in cui cadono. Il loro volume si regola con il canale **Percussioni** del mixer.

## 7. Ritmo a step

Il pulsante **Ritmo** apre un piccolo step sequencer, sempre a portata di mano anche mentre suona.

- **Attivo:** l'interruttore in alto nel pannello. Finché è spento il ritmo non suona, anche se la griglia contiene dei colpi. Ricorda di accenderlo dopo aver toccato le prime celle.
- **Passi:** 4 o 8.
- **Griglia:** quattro voci, ciascuna una riga: **Basso** (bongo grave), **Alto** (bongo acuto), **Legno** e **Vetro**. Tocca una cella per accendere o spegnere un colpo. Le celle con il bordo violetto segnano i tempi principali.
- **Informazioni:** sotto la griglia una riga riassume quanti passi hai, di che valore sono (quarti o ottavi) e a quanti BPM girano.

**Come scorre il tempo.** Un giro della griglia dura sempre **una battuta a 4/4** al BPM impostato:

- con **4 passi**, ogni passo è un quarto;
- con **8 passi**, ogni passo è un ottavo.

Per esempio a 96 BPM una battuta dura 2,5 secondi, quindi i passi durano 0,625 s (4 passi) oppure 0,31 s (8 passi).

Il ritmo ha un orologio proprio, basato sul BPM, e ogni colpo suona con l'accordo che la playhead sta attraversando in quel momento: ritmo e armonia restano quindi coerenti. Alla pressione di Play il ritmo riparte dal primo passo. Il pulsante Ritmo lampeggia a ogni colpo. Il volume si regola con il canale **Ritmo** del mixer (parte basso, al 45%, per restare accennato).

### Striscia o ritmo a step?

| | Striscia delle percussioni | Ritmo a step |
|---|---|---|
| Dove | In basso sulla lavagna | Pannello Ritmo |
| Come si crea | Si disegna | Si toccano le celle |
| Dipende da | Posizione della playhead | BPM |
| Strumenti | Cinque corsie (bongo alto e basso, legno, marimba, vetro) | Quattro voci (basso, alto, legno, vetro) |
| Mixer | Percussioni | Ritmo |

Si possono usare insieme. Se «Il BPM governa tutto» è attivo (capitolo 9), i due sistemi restano sincroni.

## 8. Armonia

### Tonalità e scala

In Impostazioni scegli **Tonalità** (una delle dodici note, oppure *Casuale*) e **Scala**:

| Scala | Carattere |
|---|---|
| **Lidio** | Luminoso e sospeso, con la quarta aumentata. |
| **Maggiore** | Stabile e solare. |
| **Misolidio** | Maggiore con la settima minore: aperto, un po' folk. |
| **Dorico** | Minore con la sesta maggiore: malinconico ma luminoso. |
| **Eolio (minore)** | Il minore naturale, più scuro. |

*Casuale* sceglie una volta all'avvio. Il pulsante **Rilancia tonalità e progressione** ne estrae una nuova (se hai fissato tonalità o scala, quelle restano).

### Progressioni e accordi

A ogni avvio, o a ogni rilancio, viene scelta una progressione di quattro accordi, uno per quarto di lavagna, tra sei possibili (gradi della scala 1-6-4-5, 1-4-1-5, 1-3-6-5, 1-5-6-4, 1-4-6-5 e 1-6-2-5). Gli accordi sono di quattro note (settime) costruite sulle note della scala, e il loro nome appare in alto.

Le note disegnate si agganciano così:

- **Drone:** fondamentale e quinta dell'accordo.
- **Arpeggio, pad e bongo:** note dell'accordo.
- **Campana:** note della scala.

### Evoluzione armonica

In Impostazioni → **Evoluzione armonica** decidi se l'armonia si muove da sola:

- **Ferma:** non cambia mai.
- **Lenta:** ogni 4 giri (è il valore predefinito).
- **Media:** ogni 2 giri.

A ogni cambio la tonica sale di una quinta, di una quarta o di un tono, quindi si resta in tonalità vicine e il passaggio suona naturale; in un caso su tre circa cambia anche la progressione. I giri si contano sulla regione di loop. **Se vuoi restare in una sola tonalità, imposta Evoluzione armonica su Ferma.**

### Griglia delle note

L'opzione «Mostra la griglia delle note» disegna sulla lavagna le note della scala; la tonica ha una riga più marcata con il suo nome e l'ottava.

## 9. Tempo, durata e BPM

Ci sono due modi di decidere la velocità.

### Modo manuale (predefinito)

- **Durata (lavagna intera):** da 6 a 90 secondi (predefinito 45). È il tempo che la playhead impiega a percorrere tutta la lavagna. Da questo dipende il suono di droni, arpeggi, campane, pad e striscia delle percussioni.
- **BPM:** governa solo il ritmo a step.

In questo modo ritmo e giro sono due orologi indipendenti. Se i loro tempi non coincidono, il ritmo si sfasa progressivamente rispetto alla playhead, come nelle musiche a fasi: può essere un effetto desiderato o no.

### Il BPM governa tutto

Sotto il cursore dei BPM c'è l'interruttore **Il BPM governa tutto**. Quando è acceso:

- la durata della lavagna si calcola dal BPM: **un giro = 4 battute a 4/4**, cioè `960 ÷ BPM` secondi;
- il cursore della durata si disattiva;
- droni, arpeggio, campane, pad, striscia delle percussioni e ritmo a step condividono lo stesso tempo: un quarto di lavagna corrisponde a una battuta, e anche a un giro completo della griglia del ritmo. Poiché partono insieme da Play, restano in fase;
- se cambi il BPM mentre suona, la velocità della playhead cambia subito.

| BPM | Durata del giro | Una battuta |
|---|---|---|
| 40 | 24 s | 6 s |
| 60 | 16 s | 4 s |
| 80 | 12 s | 3 s |
| 96 | 10 s | 2,5 s |
| 120 | 8 s | 2 s |
| 160 | 6 s | 1,5 s |

La durata del giro non scende sotto i 6 secondi: oltre 160 BPM il rapporto esatto con le battute non vale più.

Il BPM si imposta da 40 a 180.

## 10. Mixer e suono

In Impostazioni, oltre a **Volume** (generale) e **Spazio (riverbero)**, c'è un mixer con sei canali indipendenti, ciascuno da 0 a 150%:

| Canale | Cosa controlla |
|---|---|
| **Droni** | Le linee blu. |
| **Arpeggio** | Le linee viola. |
| **Campane** | Le linee ambra. |
| **Pad** | Le linee verdi. |
| **Percussioni** | I colpi disegnati nella striscia. |
| **Ritmo** | Il ritmo a step (parte al 45%). |

Tutti gli altri partono al 100%. Se i droni coprono tutto, abbassa il loro canale; se vuoi più presenza dal ritmo, alzalo. I livelli del mixer, il volume e il riverbero fanno parte delle scene (capitolo 11).

**Dietro le quinte.** Il suono è interamente sintetizzato nel dispositivo, senza campioni. Il riverbero è lungo e generato all'avvio, c'è un delay con feedback e un compressore finale che evita il clipping. La polifonia è di circa 40 voci contemporanee, oltre le quali i nuovi suoni vengono scartati.

## 11. Scene

Una **scena** è un'istantanea completa di ciò che vedi e senti: disegno, tonalità, scala e progressione, regione di loop, durata, BPM, ritmo a step, magnete, mixer, volume e riverbero. Le scene si salvano in un archivio e si richiamano con un tocco, in qualunque ordine: è pensato per un'esibizione dal vivo.

Il pulsante **Scene** apre l'elenco. Per ogni scena trovi:

| Controllo | Funzione |
|---|---|
| **+ Nuova** (in alto nel pannello) | Salva lo stato attuale come scena nuova, chiamata «Scena 1», «Scena 2» e così via. |
| **Nome** | Tocca il campo e scrivi per rinominare la scena. |
| **Richiama** | Carica la scena. |
| **Aggiorna** | Sostituisce il contenuto della scena con lo stato attuale: utile per ritoccare una scena senza crearne un'altra. |
| **Elimina** | Cancella la scena; il primo tocco chiede conferma, il secondo elimina. |

La scena richiamata per ultima resta evidenziata.

**Cosa succede al richiamo.** Il passaggio è pensato per essere fluido:

- i suoni già in corso, soprattutto i droni, sfumano con il loro rilascio naturale e si sovrappongono a quelli nuovi, senza interruzioni;
- la playhead non riparte da capo: continua dal punto in cui si trova, adattata alla regione della nuova scena;
- il disegno cambia con una breve dissolvenza;
- se stavi suonando continua a suonare, se eri fermo resti fermo.

**Consigli per l'uso dal vivo**

- Prepara le scene in anticipo, con nomi che ricordi a colpo d'occhio («Apertura», «Onde», «Chiusura»).
- Per transizioni morbide, usa scene nella stessa tonalità o in tonalità vicine: i suoni che sfumano restano consonanti con quelli nuovi.
- Imposta Evoluzione armonica su **Ferma** nelle scene dove vuoi controllare l'armonia con precisione.
- Con «Il BPM governa tutto» attivo e lo stesso BPM in tutte le scene, il tempo non cambia nei passaggi; con BPM diversi la velocità cambia al richiamo.
- Fai le prove con il dispositivo collegato all'impianto o alle cuffie reali, e tieni a portata di mano il cursore del volume generale.
- Se ritocchi una scena durante le prove, ricordati di toccare **Aggiorna**, altrimenti al prossimo richiamo ritrovi la versione salvata.

**Cosa non contiene una scena:** lo stato di Play/Stop, la posizione della playhead e le altre scene.

## 12. Salvataggio dei dati

- **Stato di lavoro.** L'app si ricorda da sola di tutto: all'apertura trovi disegno, impostazioni e tonalità come li hai lasciati.
- **Scene.** Sono in un archivio separato, che non viene toccato dallo stato di lavoro.
- **Dove sono i dati.** Restano nella memoria del browser su quel dispositivo e non vengono mai inviati in rete. Non c'è sincronizzazione fra dispositivi e non c'è ancora l'esportazione.
- **Attenzione.** Cancellare i dati dei siti web di Safari elimina anche le scene. Su iOS, un'app aggiunta alla schermata Home è in genere esente dalla pulizia automatica dei dati dei siti non usati da tempo, a differenza di una semplice scheda del browser: per questo conviene installarla.

## 13. Scorciatoie da tastiera

Utili con un computer o una tastiera collegata all'iPad.

| Tasto | Azione |
|---|---|
| **Barra spaziatrice** | Play / Stop. |
| **Cmd+Z** o **Ctrl+Z** | Annulla l'ultimo tratto. |
| **Esc** | Chiude i pannelli Ritmo, Scene e Impostazioni. |

Le scorciatoie non agiscono mentre scrivi in un campo di testo o hai selezionato un pulsante.

## 14. Idee e ricette

**Ambient lento**
Durata 60-90 secondi, scala lidia o dorica, Evoluzione lenta. Una o due linee blu spesse e lunghe nella parte bassa, qualche tratto verde (pad) a metà altezza, campane sottili in alto. Abbassa il canale Percussioni.

**Pulsazione eterea**
Attiva «Il BPM governa tutto» a 72 BPM, ritmo a 8 passi. Una griglia di partenza, dove ■ è una cella accesa:

```
Basso   ■ · · · ■ · · ·
Alto    · · · ■ · · ■ ·
Legno   · · ■ · · · · ·
Vetro   · · · · · ■ · ·
```

Poi aggiungi un drone e una linea di arpeggio sottile: tutto resta in fase.

**Arpeggio che respira**
Disegna con la Apple Pencil una linea di arpeggio premendo di più al centro e meno alle estremità: il tempo e la forza delle note cambiano lungo la linea.

**Armonia che si apre**
Con il magnete a 16 colonne, traccia una scala ascendente a gradini con le campane. Poi stringi la regione di loop sui quarti 2 e 3, per sentire come cambia il carattere con soli due accordi.

**Un set dal vivo**
Prepara quattro o sei scene nella stessa tonalità con carattere diverso (aperta, ritmica, scarna, piena). Richiamale in ordine variabile, e tra una scena e l'altra gioca con il mixer e con il riverbero.

## 15. Risoluzione dei problemi

| Problema | Cosa fare |
|---|---|
| **Non si sente nulla** | Tocca Play (l'audio parte solo dopo un tuo tocco), alza il volume del dispositivo, controlla il tasto del silenzioso sull'iPhone e i livelli del mixer. |
| **Il drone non suona** | Si sente solo mentre la playhead attraversa la linea. Controlla che la linea sia dentro la regione di loop e che il canale Droni non sia a zero. |
| **Il ritmo non parte** | Verifica che l'interruttore **Attivo** del pannello Ritmo sia acceso e che almeno una cella sia accesa. |
| **Il ritmo si sfasa rispetto al giro** | Succede quando durata e BPM sono indipendenti: accendi «Il BPM governa tutto». Se si sfasa anche con l'interruttore acceso (per esempio dopo che l'app è rimasta a lungo in secondo piano), premi Stop e poi Play per riallinearli. |
| **I disegni fuori da una zona non suonano** | Sono fuori dalla regione di loop: stringi meno le maniglie o doppio tocco sulla barra per tornare all'intera lavagna. |
| **Non riesco a disegnare in cima** | La fascia superiore è la barra del loop; disegna poco più in basso. |
| **Il suono si ferma quando blocco lo schermo** | Durante Play lo schermo resta acceso da solo; se lo spegni a mano, il sistema può sospendere l'audio. |
| **Un colpo suona due volte** | Capita se è proprio sul bordo tra la fine e l'inizio del giro: sposta il colpo di una colonna. |
| **Ho perso le scene** | Probabilmente sono stati cancellati i dati dei siti di Safari. Le scene vivono solo sul dispositivo. |
| **Vedo una versione vecchia** | Chiudi l'app dal selettore delle app e riaprila, anche due volte. Per l'aggiornamento della cache vedi il README. |

## 16. Riferimento delle impostazioni

| Impostazione | Valori | Predefinito |
|---|---|---|
| Durata (lavagna intera) | da 6 a 90 s | 45 s |
| BPM | da 40 a 180 | 96 |
| Il BPM governa tutto | acceso / spento | spento |
| Regione di loop | maniglie sulla barra | intera lavagna |
| Tonalità | Casuale oppure una delle 12 note | Casuale |
| Scala | Casuale, lidio, maggiore, misolidio, dorico, eolio | Casuale |
| Evoluzione armonica | Ferma, Lenta (4 giri), Media (2 giri) | Lenta |
| Griglia ritmica (striscia) | Libera, 32, 64, 128 passi per giro | 64 |
| Griglia magnetica | 8, 16, 32, 64, 128 colonne | 16 (magnete spento) |
| Volume | da 0 a 100% | 70% |
| Spazio (riverbero) | da 0 a 100% | 60% |
| Mixer (sei canali) | da 0 a 150% | 100%, Ritmo 45% |
| Mostra la griglia delle note | sì / no | sì |
| Ritmo a step | Attivo sì/no, 4 o 8 passi | spento, 8 passi |
| Spessore del tratto | da sottile a spesso | medio |
