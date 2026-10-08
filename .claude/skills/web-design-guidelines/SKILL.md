# Web Design Guidelines

Reviews UI/HTML/CSS code against web best practices: accessibility, UX, visual hierarchy, responsive design.

## Quando usarla
Invoca questa skill ogni volta che vuoi un audit su un file HTML/CSS prima di andare live. Utile per aruggiero.com, impronta-sito-concept.html, qualsiasi nuova pagina.

## Come procedere
1. Fetch le linee guida aggiornate da: https://raw.githubusercontent.com/vercel-labs/agent-skills/main/skills/web-design-guidelines/SKILL.md
2. Leggi i file specificati dall'utente (o chiedi quali file analizzare)
3. Controlla ogni file contro le regole fetchate
4. Riporta i problemi nel formato `file:riga — problema`
5. Priorità: [BLOCCO] problemi critici / [AVVISO] miglioramenti / [SUGGERIMENTO] ottimizzazioni

## Checklist minima da verificare sempre
- `lang` attribute su `<html>`
- Meta viewport presente
- Alt text su tutte le immagini
- Contrasto colori sufficiente (WCAG AA)
- Nessun testo sotto 12px
- Link con testo descrittivo (non "clicca qui")
- Layout funzionante a 375px (mobile)
- Nessun overflow orizzontale
- Font caricato con `font-display: swap`

## Non fare
- Non suggerire framework se il sito è statico HTML
- Non introdurre dipendenze esterne senza giustificazione
