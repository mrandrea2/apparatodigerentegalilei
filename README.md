# BioLab · L’apparato digerente

Web app didattica interattiva per il Liceo scientifico a indirizzo sportivo Galilei di Verona.

**A cura del prof. Andrea Bertelli**

## Funzionalità

- Atlante anatomico interattivo con 7 strutture selezionabili.
- 5 unità di apprendimento avanzato e domande di ripasso.
- Simulatore dei processi digestivi per carboidrati, proteine e lipidi.
- Caso studio sportivo con scelta di ipotesi fisiologiche.
- Quiz di 12 domande con risposta spiegata, risultato e revisione.
- Glossario scientifico ricercabile.
- Salvataggio locale delle unità completate nel browser.
- Interfaccia responsive, sfondi chiari e testo scuro.

## Requisiti

Node.js 20.19+ o 22.12+ e npm.

## Avvio sul computer

```bash
npm install
npm run dev
```

Apri l'indirizzo mostrato nel terminale (generalmente `http://localhost:5173`).

## Creare la build

```bash
npm run build
npm run preview
```

La cartella `dist` contiene il sito pronto per la distribuzione.

## Pubblicare su GitHub

1. Crea un repository vuoto su GitHub (es. `apparato-digerente-galilei`).
2. Entra nella cartella del progetto e avvia:

```bash
git init
git add .
git commit -m "Prima versione BioLab apparato digerente"
git branch -M main
git remote add origin https://github.com/TUO-USERNAME/apparato-digerente-galilei.git
git push -u origin main
```

Sostituisci `TUO-USERNAME` con il tuo username GitHub. Se GitHub richiede autenticazione, usa il metodo di accesso configurato sul tuo computer (browser o token).

## Pubblicare su Vercel

1. Accedi a [vercel.com](https://vercel.com), autenticandoti con GitHub.
2. Seleziona **Add New → Project**, poi importa il repository.
3. Il framework Vite viene rilevato automaticamente.
4. Controlla che il comando di build sia `npm run build` e la directory di output `dist`.
5. Premi **Deploy**.

Le modifiche successive inviate sul branch collegato genereranno nuove distribuzioni automatiche.

## Organizzazione file

```
├── index.html       # Pagina HTML principale
├── package.json     # Script e dipendenze
├── vercel.json      # Configurazione Vercel
├── src/
│   ├── main.jsx     # Interfaccia e interazioni
│   ├── data.js      # Contenuti scientifici e quesiti
│   └── style.css    # Stile responsive
└── README.md
```

## Personalizzazione

- **Contenuti**: modifica `src/data.js`.
- **Quiz**: aggiorna l'array `questions` in `src/data.js`.
- **Grafica**: modifica `src/style.css`.
- **Intestazione, pagine e funzioni**: modifica `src/main.jsx`.

## Note didattiche

I disegni anatomici sono schemi semplificati e non sono in scala. Il caso sportivo è destinato all'apprendimento dei meccanismi, non a fornire prescrizioni individuali. I progressi si conservano solo nel browser del dispositivo in uso; non vengono raccolti nominativi o risultati degli studenti su un server.

Riferimenti di approfondimento: [NIDDK](https://www.niddk.nih.gov/health-information/digestive-diseases/digestive-system-how-it-works), [NCBI Bookshelf – Physiology, digestion](https://www.ncbi.nlm.nih.gov/books/NBK544242/).
