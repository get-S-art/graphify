# Brand Consistency — Artur Ruggiero

Applica e verifica il design system di Artur su qualsiasi HTML/CSS generato. Va invocata AUTOMATICAMENTE ogni volta che si crea o modifica un file per aruggiero.com, impronta, carospite, o qualsiasi progetto visivo di Artur.

## Design System completo

### Typography
- Font unico: **Bricolage Grotesque** (Google Fonts)
- Import: `<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,200..800&display=swap" rel="stylesheet">`
- Body: 400, heading: 700-800, accent: 200

### Palette (CSS custom properties)
```css
:root {
  --blu: #1C4EE4;
  --rosa: #EA308C;
  --teal: #34B9AF;
  --bianco: #ffffff;
  --nero: #0a0a0a;
  --grigio: #f5f5f5;
}
```

### Maschere petalo
```css
.petalo {
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
/* Sfondo decorativo: opacity 0.15-0.2, mai coprente il contenuto */
```

### Animazioni
```css
@keyframes floatDrop {
  0% { opacity: 0; transform: translateY(-20px); }
  100% { opacity: 1; transform: translateY(0); }
}
/* Usa IntersectionObserver per reveal on scroll */
```

### Regole strutturali (NON NEGOZIABILI)
1. HTML statico self-contained — CSS inline, no framework, no build step
2. Immagini: max 1000px lato lungo, 72% qualità JPEG, embedded base64
3. Footer: link testuali, zero icone SVG
4. CTA unica funnel: "inizia con il check-up →" → /check-up
5. Niente date eventi visibili
6. Mix masonry per contenuti (foto + testo + quote nello stesso flusso)

### Voce del copy (solo se generi testo)
- Nessuna lineetta "—" nel testo
- Nessuna frase che inizia con "Non" / "Né" / "Mai"
- Periodi del corpo ≥ 15 parole
- Zero pattern AI: "Eccoci al punto:", "la verità è che:"

## Checklist automatica prima di consegnare HTML
- [ ] Font Bricolage Grotesque caricato
- [ ] Palette usa variabili CSS --blu --rosa --teal
- [ ] Maschere petalo presenti dove previste dal design
- [ ] Nessun framework introdotto
- [ ] CSS inline nel file
- [ ] Immagini compresse e base64 se necessario
