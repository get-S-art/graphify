# Playwright Browser Testing

Testa automaticamente il sito aprendo un browser reale. Verifica che ogni modifica funzioni visivamente senza aprire Chrome a mano.

## Quando usarla
Dopo ogni modifica significativa a HTML/CSS, prima di dichiarare il lavoro finito. Obbligatoria prima di qualsiasi deploy.

## Prerequisiti
```bash
npm install -g @playwright/test playwright-cli
playwright-cli install --skills
```

## Come procedere
1. Avvia una sessione: `playwright-cli open -s=test`
2. Naviga al file o URL: `playwright-cli goto file:///path/to/index.html -s=test`
3. Prendi snapshot: `playwright-cli snapshot -s=test` → salva riferimento visivo
4. Fai click e interazioni: `playwright-cli click [id] -s=test`
5. Verifica mobile: ridimensiona a 375px e ri-snapshot
6. Screenshot finale: `playwright-cli screenshot -s=test`

## Checklist pre-deploy per siti di Artur
- [ ] Homepage carica senza errori console
- [ ] CTA "inizia con il check-up →" è visibile e cliccabile
- [ ] Maschere petalo si renderizzano correttamente
- [ ] Animazioni reveal funzionano allo scroll
- [ ] Layout mobile 375px non ha overflow
- [ ] Font Bricolage Grotesque caricato
- [ ] Nessuna immagine rotta

## Configurazione headless
Di default gira headless. Per vedere il browser: aggiungi `--headed` ai comandi.
