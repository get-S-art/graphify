# Taste Skill — Visual Design Quality Control

Valuta la qualità estetica di un UI generato. Simula il giudizio di un designer esperto su equilibrio visivo, gerarchia, coerenza, "taste".

## Quando usarla
Dopo aver generato HTML/CSS, prima di mostrarlo all'utente. Chiediti: "questo sembra fatto da un designer o da una macchina?"

## Come procedere
1. Guarda il design generato come se fossi un art director
2. Valuta su 5 dimensioni:
   - **Gerarchia visiva**: l'occhio sa dove andare?
   - **Spazio negativo**: c'è respiro o tutto è compresso?
   - **Coerenza**: font, colori, spaziature seguono un sistema?
   - **Autenticità**: sembra un sito reale o un template generico?
   - **Mobile**: funziona con dignità a 375px?
3. Per ogni problema: nomina il problema, spiega perché è un problema, proponi la fix specifica

## Anti-pattern da flaggare immediatamente
- Gradiente viola/blu AI generico → sostituisci con la palette di Artur
- Cards dentro cards dentro cards → semplifica la struttura
- Troppe sezioni hero → massimo 1 hero, poi contenuto
- Font size identico ovunque → stabilisci scala tipografica chiara
- Bottoni generici "Click here" o "Learn More" → copy specifico
- Ombre ovunque → usa l'ombra come strumento, non decorazione
- Animazioni su tutto → meno è più

## Output atteso
Un giudizio breve e diretto: cosa funziona, cosa non funziona, fix prioritari.
Non una lista di 20 punti — massimo 5 fix, ordinate per impatto.
