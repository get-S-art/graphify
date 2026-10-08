# Image to Code

Converte un'immagine (screenshot, mockup, foto di wireframe su carta) in codice HTML/CSS funzionante.

## Quando usarla
Quando l'utente fornisce un'immagine come riferimento visivo per una pagina o componente. Evita cicli lunghi di spiegazione testuale.

## Come procedere
1. Analizza l'immagine in dettaglio: testo visibile, tipografia, spaziatura, bottoni, colori, layout
2. Identifica le sezioni principali e la gerarchia visiva
3. Implementa sezione per sezione, non tutta in una volta
4. Genera una sezione alla volta con preview mentale della fedeltà
5. Verifica che il risultato rispetti le proporzioni dell'originale

## Regole per il design system di Artur
Se il target è aruggiero.com o qualsiasi progetto Artur, applica automaticamente:
- Font: Bricolage Grotesque (Google Fonts)
- Palette: --blu: #1C4EE4 / --rosa: #EA308C / --teal: #34B9AF / sfondo: #ffffff
- Maschere petalo: `border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%`
- Animazioni reveal: IntersectionObserver con keyframe floatDrop
- CSS inline, no framework, no build step

## Anti-pattern da evitare
- Niente nested cards dentro cards
- Niente gradiente viola generico AI
- Niente filler copy inventato
- Non tagliare le immagini (usa `aspect-ratio: auto`)
