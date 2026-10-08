# SEO Audit

Verifica completa dell'indicizzabilità di un sito. Identifica tutto ciò che impedisce a Google e Brave di trovare le pagine.

## Quando usarla
Ogni volta che un sito non appare nei risultati di ricerca, prima di qualsiasi lavoro SEO, e come checklist mensile di controllo.

## Come procedere

### Step 1 — Blocchi critici (risolvono il 90% dei problemi)
1. Controlla `robots.txt` su `[dominio]/robots.txt` — cerca `Disallow: /` o `User-agent: *\nDisallow: /`
2. Per WordPress: verifica Impostazioni → Lettura → spunta su "Scoraggia i motori di ricerca" = BLOCCO CRITICO
3. Controlla ogni pagina per `<meta name="robots" content="noindex">`
4. Verifica se esiste `sitemap.xml` su `[dominio]/sitemap.xml`

### Step 2 — Structured Data
5. Verifica presenza JSON-LD nella head (`<script type="application/ld+json">`)
6. Controlla che i tipi siano corretti (Person, WebSite, LocalBusiness secondo il caso)
7. Testa con Google Rich Results Test

### Step 3 — Meta essenziali
8. `<title>` — presente, unico per pagina, 50-60 caratteri
9. `<meta name="description">` — presente, 150-160 caratteri
10. `<meta property="og:title">` e `og:description` — per social sharing
11. `<link rel="canonical">` — punta a sé stesso (evita duplicati)

### Step 4 — Performance che impatta SEO
12. Tempo caricamento < 3 secondi (soprattutto mobile)
13. Nessuna immagine > 500KB senza compressione
14. Font con `font-display: swap`

## Riporta i risultati così
**[BLOCCANTE]** — impedisce completamente l'indicizzazione → risolvi subito
**[IMPORTANTE]** — riduce visibilità → risolvi questa settimana
**[OTTIMIZZAZIONE]** — migliora ranking → risolvi nel prossimo sprint

## Per aruggiero.com specificamente
- Verifica il blocco WordPress (Impostazioni → Lettura)
- Controlla che il JSON-LD Person sia corretto con nome, URL, sameAs LinkedIn
- Sitemap deve includere home + /my-work + /thinking-about-me + /check-up
