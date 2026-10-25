# S33 - Loopscape

Strumento musicale generativo per iPad e iPhone, in forma di app web installabile (PWA). Disegni linee e punti su una lavagna bianca; una playhead che gira in loop li trasforma in droni, arpeggi, campane, pad e percussioni, sempre intonati secondo le regole dell'armonia. Pensato per l'ambient, anche dal vivo.

Fa parte della famiglia di strumenti **S33**.

**Prova subito:** <https://satarsa33.github.io/s33_Loopscape/>

<!-- Aggiungi qui uno screenshot, ad esempio: ![Loopscape](docs/screenshot.png) -->

## Cosa fa

- **Disegni, lui suona.** L'altezza del tratto è l'altezza della nota, il colore è il timbro, lo spessore è intensità e durata.
- **Armonia automatica.** Ogni quarto della lavagna ha il suo accordo; le note si agganciano alla scala e all'accordo, quindi qualsiasi scarabocchio resta intonato. Tonalità e scala si scelgono o escono a caso, e possono evolvere da sole verso tonalità vicine.
- **Quattro strumenti disegnabili:** drone, arpeggio, campana, pad.
- **Striscia ritmica** in basso, con cinque corsie (bongo alto, bongo basso, legno, marimba, vetro) dove i colpi si disegnano e si ripetono a ogni giro.
- **Step sequencer** minimale a 4 o 8 passi, a griglia visibile e modificabile, sincronizzato a un BPM.
- **Loop di una regione:** due maniglie sulla barra in cima restringono il giro a una parte della lavagna.
- **Griglia magnetica** per tracciare linee precise.
- **Mixer** a sei canali, volume generale e riverbero.
- **Scene:** archivio di composizioni complete (disegno e impostazioni) da richiamare in qualsiasi ordine, pensato per l'uso dal vivo.
- **Funziona offline** dopo il primo caricamento e tiene lo schermo acceso durante la riproduzione.
- **Nessuna dipendenza, nessun tracciamento:** un solo file HTML, tutto il suono è sintetizzato in tempo reale, i dati restano sul dispositivo.

La guida completa è nel [Manuale](MANUALE.md).

## Avvio rapido

1. Apri la pagina e tocca **Play**.
2. Scegli un colore in basso e disegna sulla lavagna.
3. Tocca una linea o un punto nella **striscia viola** in basso per aggiungere percussioni.
4. Apri **Impostazioni** (icona con i cursori, in alto a destra) per durata, BPM, tonalità e mixer.

Su iPhone e iPad il suono parte solo dopo il primo tocco su Play, per una regola di iOS.

## Installare l'app su iPad o iPhone

1. Apri l'indirizzo in **Safari**.
2. Tocca **Condividi** e poi **Aggiungi alla schermata Home**.
3. Si apre a schermo intero, come un'app, e funziona anche senza rete.

## Struttura del repository

```
index.html              l'app (HTML, CSS e JavaScript in un unico file)
manifest.webmanifest    nome, colori e icone per l'installazione
sw.js                   service worker: cache per l'uso offline
icons/
  apple-touch-icon.png
  favicon-32.png
  icon-192.png
  icon-512.png
  icon-maskable-512.png
README.md
MANUALE.md
```

## Pubblicare su GitHub Pages

1. Carica i file nella **radice** del repository, con `index.html` in cima e la cartella `icons` accanto (non dentro un'altra cartella e non come file `.zip`).
2. Vai in **Settings → Pages**, scegli il ramo (di solito `main`) e la cartella `/ (root)`, poi salva.
3. Attendi uno o due minuti: l'indirizzo sarà `https://<utente>.github.io/<repository>/`.

I nomi dei file distinguono maiuscole e minuscole: devono essere scritti esattamente come sopra. L'app usa solo percorsi relativi, quindi funziona anche in una sottocartella.

## Sviluppo in locale

Non c'è nessuna fase di build. Per provare l'app serve un piccolo server, perché il service worker funziona solo su `http://localhost` o su HTTPS:

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```

## Pubblicare un aggiornamento

Il service worker risponde dalla cache e aggiorna in background, quindi la versione nuova compare al lancio successivo. Per forzare la distribuzione di una modifica, cambia il numero di versione in `sw.js`:

```js
const CACHE = 'loopscape-v10';   // incrementa a ogni rilascio, ad esempio v11
```

## Note tecniche

- **Audio:** Web Audio API. Droni, arpeggi, campane, pad e percussioni sono sintetizzati con oscillatori, filtri e rumore; non ci sono file audio. Il riverbero è a convoluzione, con risposta all'impulso generata all'avvio. In coda ci sono un delay con feedback e un compressore.
- **Disegno:** due canvas sovrapposti (tratti e animazioni), eventi Pointer, pressione della Apple Pencil, rifiuto del palmo (i tocchi nel secondo e mezzo successivo alla penna vengono ignorati).
- **Dati:** `localStorage`. Lo stato di lavoro si salva da solo; le scene sono in una chiave separata. Nulla viene inviato in rete.
- **Polifonia:** circa 40 voci contemporanee, oltre le quali i nuovi suoni vengono scartati.
- **Tema:** l'interfaccia segue il tema chiaro o scuro del sistema; la lavagna resta bianca.

## Limiti noti

- Le scene e il salvataggio sono locali a ogni dispositivo e a ogni browser: non c'è sincronizzazione né esportazione.
- Sopra i 160 BPM, con «Il BPM governa tutto» attivo, la durata del giro si ferma al minimo di 6 secondi e il rapporto esatto con le battute non vale più.
- Nel passaggio esatto tra la fine e l'inizio del giro, un colpo posizionato sul bordo può suonare due volte a breve distanza.
- Su iOS un'app aggiunta alla Home è in genere esente dalla pulizia automatica dei dati dei siti non usati da tempo, a differenza di una semplice scheda di Safari.
- Non c'è ancora la registrazione dell'audio.

## Idee in valutazione

Altri strumenti nella striscia ritmica (shaker, tamburello), esportazione e importazione delle scene, registrazione dell'audio.

## Se qualcosa non funziona

- **Pagina bianca o errore 404:** controlla di aver caricato i file singoli nella radice del repository e che Pages sia attivo su quel ramo.
- **Nessun suono:** tocca prima Play, alza il volume del dispositivo e controlla il tasto del silenzioso sull'iPhone.
- **Vedi una versione vecchia:** chiudi l'app dal selettore delle app e riaprila (a volte due volte). Se persiste, su iPad vai in Impostazioni → Safari → Avanzate → Dati dei siti web ed elimina il sito. Ricorda che cancellare i dati elimina anche le scene salvate.
- **Il nome o l'icona non cambiano sulla Home:** rimuovi l'app e aggiungila di nuovo.

## Licenza

Da definire: aggiungi un file `LICENSE` al repository prima di condividere il codice.
