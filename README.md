# 🎩 I Sei Cappelli di Claude

> *Separare i contesti per pensare meglio, ispirato ai Sei Cappelli di Edward De Bono*

**by [Vicius Lio](https://www.linkedin.com/in/vincenzo-lio-dataengineer/)**

---

## Il problema

Usiamo Claude come se fosse un unico strumento per tutto. Un'email professionale, poi Heidegger, poi un bug in produzione, poi cosa cucinare stasera. Claude risponde a tutto, ma senza contesto, senza sapere chi stai cercando di essere in quel momento, le risposte sono mediocri. Non perché Claude sia mediocre. Perché l'input è sbagliato.

## La soluzione: i Cappelli

Su Claude puoi creare **Progetti** (workspace separati con istruzioni persistenti). Ogni Progetto è un cappello. Ogni cappello ha un contesto preciso, un tono calibrato, regole specifiche.

La differenza pratica è quella che c'è tra parlare con qualcuno che ti conosce e qualcuno a cui devi sempre spiegare tutto da capo.

---

## I sei cappelli

| # | Cappello | Contesto |
|---|----------|----------|
| 🔵 | [**Lavoro**](hats/01-work/) | Produttività professionale, codice, architetture, email, report |
| 🟣 | [**Mente**](hats/02-mind/) | Esplorazione intellettuale, filosofia, letture, idee |
| 🟡 | [**Creativo**](hats/03-creative/) | Progetti creativi, scrittura, musica, arte |
| 🟢 | [**Personale**](hats/04-personal/) | Vita familiare, relazioni, decisioni personali |
| 🔴 | [**Benessere**](hats/05-wellness/) | Sport, salute, alimentazione, routine |
| ⚪ | [**Finanze**](hats/06-finance/) | Investimenti, budget, pianificazione economica |

---

## Come usare questa repo

### Opzione A: Usa un cappello già pronto
1. Scegli il cappello che ti serve dalla cartella `hats/`
2. Apri `instructions.md` e personalizza i placeholder `[...]`
3. Su Claude → **Nuovi Progetti** → incolla il testo nelle istruzioni del progetto
4. Usa i prompt in `templates.md` per iniziare subito

### Opzione B: Costruisci il tuo cappello
1. Leggi [`meta/how-to-build-a-hat.md`](meta/how-to-build-a-hat.md) per capire la logica
2. Usa [`meta/hat-template.md`](meta/hat-template.md) come punto di partenza
3. Personalizza in base al tuo contesto

---

## Regole d'uso del sistema

| Regola | Dettaglio |
|--------|-----------|
| **Una chat, un task** | Non mescolare cappelli diversi. Nuova chat = nuovo contesto. |
| **Chat corte** | Apri una nuova chat spesso (il context rot è reale). |
| **Istruzioni sotto 500 parole** | Ogni parola in più è un token in meno per il lavoro vero. |
| **Cappelli come strumenti, non identità** | Sono modalità temporanee, non personalità rigide. |

---

## Limiti noti

Questo sistema è un'ispirazione ai Sei Cappelli di De Bono, non un'implementazione fedele. De Bono usava i cappelli come stati temporanei; questa implementazione rischia di renderli identità fisse. Tienilo a mente.

Le istruzioni consumano token. Mantienile concise: massimo 400-500 parole per cappello.

Il sistema non risolve il context rot, lo sposta per contesto. Apri nuove chat frequentemente.

---

## Struttura della repo

```
six-hats-claude/
├── README.md
├── meta/
│   ├── how-to-build-a-hat.md    # Guida per creare un cappello personalizzato
│   └── hat-template.md          # Template vuoto da cui partire
└── hats/
    ├── 01-work/
    │   ├── instructions.md      # Testo da incollare nelle istruzioni del Progetto
    │   └── templates.md         # Prompt pronti all'uso
    ├── 02-mind/
    ├── 03-creative/
    ├── 04-personal/
    ├── 05-wellness/
    └── 06-finance/
```

---

## Contribuire

Hai un cappello che funziona bene e vuoi condividerlo? Apri una PR con la struttura standard (`instructions.md` + `templates.md`) nella cartella `hats/`. Generalizza sempre i placeholder: questa repo serve a chiunque, non solo a te.

---

## Articolo

L'idea dietro questo sistema è spiegata nell'articolo [*I sei cappelli di Claude*](https://medium.com/@viciuslios/i-sei-cappelli-di-claude-6a648056e45f) pubblicato su Medium.

---

*Ispirato ai Six Thinking Hats di Edward De Bono (1985).*
