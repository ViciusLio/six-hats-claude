# Come costruire il tuo cappello

Un cappello efficace non è una lista di cose che Claude deve sapere. È la risposta a una domanda precisa: **chi sei tu in questo contesto, e cosa ti serve da un interlocutore intelligente?**

---

## Le cinque domande

Prima di scrivere una sola riga di istruzioni, rispondi a queste:

1. **Chi sei in questo contesto?** — ruolo, livello di esperienza, responsabilità
2. **Con chi interagisci?** — colleghi, clienti, studenti, partner, te stesso
3. **Quali output produci?** — codice, email, analisi, decisioni, idee
4. **Cosa non deve mai succedere?** — dati sensibili esposti, tono sbagliato, scelte rischiose senza alert
5. **Come vuoi che ti risponda?** — tono, lunghezza, formato, lingua

---

## La struttura standard

Ogni cappello è composto da cinque blocchi. Usali tutti, nell'ordine che preferisci.

### Blocco 1 — Identità e contesto
Chi sei, cosa fai, con chi lavori. Massimo 5 righe. Più specifico sei, migliore è il comportamento del modello.

```
Sei il mio assistente [professionale / creativo / personale].
- Ruolo: [descrivi il tuo ruolo o il contesto di vita]
- Interlocutori: [con chi interagisci in questo contesto]
- Output frequenti: [lista dei 3-5 output principali]
```

### Blocco 2 — Tono e stile
Come vuoi che ti risponda. Non lasciarlo al caso — Claude si adatta molto bene se gli dici cosa vuoi.

```
- Tono: [diretto / empatico / tecnico / esplorativo / ...]
- Profondità: [adatta all'interlocutore / sempre alta / sempre accessibile]
- Lingua: [italiano / inglese / adatta al contesto]
- Lunghezza risposte: [concise / dettagliate / dipende dal task]
```

### Blocco 3 — Formato output (per cappelli tecnici o produttivi)
Se produci output strutturati (codice, analisi, email), definisci cosa vuoi sempre ricevere.

```
Per ogni output [codice / analisi / documento] fornisci:
1. L'output richiesto
2. Il perché di quella scelta
3. Almeno un'alternativa
4. Una domanda di verifica
```

### Blocco 4 — Guardrail
Cosa non deve mai fare senza prima dirtelo. Questa sezione protegge il tuo contesto.

```
Se rilevi [rischio X / scelta rischiosa / dato sensibile]:
→ NON procedere in silenzio. Chiedimi conferma esplicita.
Marca con ⚠️ DA VERIFICARE: [lista output critici]
```

### Blocco 5 — Regola meta
Tiene i cappelli separati. Sostituisci "questo cappello" con il nome che hai dato al progetto.

```
Questo è il Cappello [NOME]. Se mi chiedi qualcosa chiaramente
fuori contesto, ricordami gentilmente che ho un progetto dedicato.
```

---

## Checklist prima di pubblicare

- [ ] Le istruzioni sono sotto le 500 parole?
- [ ] Hai rimosso tutti i dati personali identificativi?
- [ ] I placeholder `[...]` sono chiari per chi non ti conosce?
- [ ] Il tono descritto è davvero quello che vuoi in questo contesto?
- [ ] Hai testato le istruzioni con almeno 3 prompt diversi?

---

## Errori comuni

**Istruzioni troppo lunghe** — ogni parola è un token. Taglia tutto quello che non cambia concretamente il comportamento del modello.

**Mescolare più contesti** — se ti viene voglia di aggiungere "e quando parlo di X allora..." stai cercando di costruire due cappelli in uno. Crea un secondo cappello.

**Cappello come identità fissa** — i cappelli sono strumenti temporanei, non personalità. Se il tuo cappello Lavoro inizia a risponderti anche sui weekend, hai un problema di configurazione (o di dipendenza).

**Nessun guardrail** — specialmente per cappelli che gestiscono output critici (email a clienti, codice da deployare, decisioni finanziarie), definisci sempre cosa deve bloccarsi e chiederti conferma.
