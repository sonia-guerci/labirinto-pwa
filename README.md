# Labirinto PWA

Un semplice gioco da realizzare in classe sotto forma di PWA.

Il progetto è un labirinto interattivo in cui il giocatore deve partire dal punto di inizio e raggiungere l'obiettivo senza uscire dal percorso. Il gioco misura il tempo impiegato, tiene traccia del miglior record e può essere installato come applicazione web progressiva (PWA).

## Funzionalità

- Labirinto SVG interattivo
- Timer in tempo reale
- Livelli di difficoltà: facile, medio, difficile
- Salvataggio del miglior tempo con `localStorage`
- Supporto PWA con service worker e manifest
- Compatibilità con desktop e dispositivi mobili

## Anteprima

Il gioco è costruito con HTML, CSS e JavaScript vanilla, senza framework esterni.

## Struttura del repository

- `index.html` — struttura del gioco e logica di interazione
- `manifest.json` — configurazione della PWA
- `sw.js` — service worker per la cache e l'installazione dell'app
- `logo.svg` — logo dell'app
- `favicon.svg` — icona del sito

## Come eseguire il progetto

Per il corretto funzionamento del service worker e delle funzionalità PWA, è consigliato avviare il progetto tramite un server locale.

### Live Server di Visual Studio Code

1. Installa l'estensione **Live Server** in Visual Studio Code.
2. Apri la cartella del progetto.
3. Fai clic con il tasto destro su `index.html`.
4. Seleziona **Open with Live Server**.

Il progetto verrà aperto automaticamente nel browser, generalmente su un indirizzo simile a:

```text
http://127.0.0.1:5500
```

### PHP Live Server

Se hai PHP installato, puoi avviare un server locale dalla cartella del progetto con:

```bash
php -S localhost:8000
```

Poi apri nel browser:

```text
http://localhost:8000
```

### XAMPP

1. Copia la cartella `labirinto-pwa` nella directory `htdocs` di XAMPP.
2. Avvia **Apache** dal pannello di controllo di XAMPP.
3. Apri nel browser:

```text
http://localhost/labirinto-pwa
```

## Come giocare

1. Posizionati sul cerchio di partenza (`START`).
2. Esci dal cerchio per far partire il timer.
3. Muoviti lungo il percorso oscuro senza uscire dal tracciato.
4. Arriva al cerchio di arrivo (`GOAL`).
5. Se esci dal percorso, perdi la partita.
6. Il miglior tempo viene salvato automaticamente nel browser.

## PWA

Il progetto include:

- `manifest.json` per definire il nome, i colori e l'icona
- `sw.js` per gestire la cache e consentire l'uso offline

Per installare la PWA, apri la pagina in un browser moderno tramite un server locale e usa l'opzione **Installa app** o **Add to Home Screen**, quando disponibile.

## TODO / Possibili miglioramenti

- aggiungere più livelli o labirinti
- aggiungere suoni e animazioni
- migliorare l'accessibilità
- introdurre un sistema di punteggio e classifiche

## Licenza

Questo progetto non include un file di licenza esplicito. Se vuoi, puoi aggiungerne uno in base al tuo utilizzo (ad esempio MIT o CC BY-SA).

## Autore

Creato come progetto didattico per essere realizzato in classe.
