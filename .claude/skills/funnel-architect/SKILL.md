# Funnel Architect — Business di Artur

Conosce il modello di business completo di Artur. Va caricata quando si costruiscono automazioni, form, email sequence, CRM, integrazioni API legate al funnel di acquisizione clienti.

## Il funnel in 5 stadi

1. **Check-up** (form diagnostico su /check-up)
   - 27 campi, stile Illogician
   - Layout: 2 colonne desktop, stack mobile
   - CTA: "inizia con il check-up →"
   - Sottotitolo: "15 minuti. Un report gratuito in 48h. Poi decidi tu."

2. **Triage AI** (Claude API → referto automatico)
   - Tool: Claude API con prompt Illogician dedicato
   - Pipeline: Form → webhook → Claude API → output "sintomi grezzi"
   - Revisione manuale Artur (10-15 min) → invio via email

3. **Call 1** (gratuita, 30 min)
   - Obiettivo: build rapport + diagnosi fit
   - Booking: Calendly
   - Output: decide se proseguire

4. **Call 2 Diagnostica** (€1.000)
   - Deliverable: mini-report in 48h + next steps
   - Questo è il primo revenue touchpoint

5. **Retainer mensile** (€1.200/mese)
   - Embedded nel business del cliente
   - Obiettivo: €2.000/mese netti

## Stack tecnico autorizzato
- Form: Tally (gratis) o Typeform (~30€/mese)
- Pipeline: n8n (self-hosted) o Make (~30€/mese)
- Email: Resend (gratis fino a soglie basse)
- CRM: Notion o Airtable (gratis)
- Calendly per booking
- Costo totale: 30-160€/mese

## Regole per le automazioni
1. Fase 1 (primi 10 form): AI produce draft, Artur revisiona
2. Fase 2 (form 11+): AI automatizzata, Artur quality control
3. Fase 3 (30+ form/mese): AI autonoma, Artur solo su output anomali
4. Mai hardcode di API key — variabili d'ambiente sempre
5. Testare sempre con form finto prima di andare live

## Clienti attivi da tenere in mente
- **Impronta S.C.S** (Chioggia) — Artur è amministratore, progetto da avviare
- **Capatoast** — prospect, Call 1 completata, Call 2 ancora da fare

## Linguaggio vietato nei copy del funnel
Niente "anamnesi", "diagnosi", "clinica" — usa "domanda giusta", "check-up", "referto strategico"
