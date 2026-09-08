# Amsterdam Field Guide — GitHub Pages

Questa cartella è pronta per GitHub Pages.

## Pubblicazione più semplice

1. Su GitHub crea un nuovo repository, ad esempio `amsterdam-guide`.
2. Impostalo **Public** se vuoi usare GitHub Pages gratuitamente senza vincoli di visibilità.
3. Carica **tutti i file di questa cartella nella root del repository**:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
4. Apri il repository → **Settings** → **Pages**.
5. In **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
6. Salva.

GitHub mostrerà l'indirizzo pubblico, normalmente:
`https://TUO-USERNAME.github.io/amsterdam-guide/`

## Condivisione

Invia quel link via WhatsApp. Il destinatario non deve avere GitHub.

## Installazione su iPhone

Apri il link con Safari → pulsante Condividi → **Aggiungi alla schermata Home**.

L'app si aprirà poi in modalità standalone, senza la normale barra del browser.

## Offline

Dopo il primo caricamento online, i file principali dell'app vengono memorizzati dal service worker.
Le sezioni interne resteranno disponibili anche senza rete.  
Google Maps, siti dei locali, biglietti e servizi esterni richiedono invece connessione.

## Aggiornare la guida

Sostituisci `index.html` nel repository e fai Commit. GitHub Pages pubblicherà la nuova versione.
Se modifichi anche il service worker, cambia ad esempio `ams-guide-v1` in `ams-guide-v2` dentro `sw.js`
per forzare l'aggiornamento della cache.
