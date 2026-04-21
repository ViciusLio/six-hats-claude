# I sei cappelli di Claude (quando separare i contesti aiuta a pensare meglio)

*by Vicius Lio*

---

Nel 1985 Edward De Bono pubblicò un libro sottile con un titolo bizzarro. *Six Thinking Hats* — Sei cappelli per pensare. L'idea era semplice: il problema del pensiero non è la mancanza di intelligenza, è che mescoliamo tutto. Emozioni, dati, critiche, idee nuove, ottimismo e pessimismo finiscono nello stesso calderone mentre discutiamo, e il risultato è quello che conoscete: riunioni che non decidono niente, idee che muoiono sotto il peso delle obiezioni prima ancora di essere esplorate.

De Bono propose una soluzione elegante. Sei cappelli colorati, ognuno con un modo di pensare preciso. Il cappello bianco guarda solo i dati. Il rosso porta le emozioni. Il nero è la critica. Il giallo l'ottimismo. Il verde la creatività. Il blu gestisce il processo. L'idea non era di indossarli tutti insieme, era di indossarli uno alla volta, così che ogni tipo di pensiero avesse il suo spazio senza interferire con gli altri.

Il libro diventò un classico del management, anche se vale la pena dirlo con onestà: le prove che il metodo produca miglioramenti misurabili nel pensiero sono scarse. De Bono era più interessato all'utilità pratica delle sue idee che a dimostrarne scientificamente l'efficacia. Non è un difetto — è una scelta di campo. Il metodo funziona perché funziona nella pratica, non perché lo dice uno studio controllato.

Decenni dopo, quasi inconsapevolmente, ho ritrovato la stessa logica mentre cercavo di capire come usare Claude in modo sensato.

---

Il problema con l'AI non è l'AI.

È che la usiamo come se fosse un unico strumento per tutto. Una chat generica dove oggi chiedo di riscrivere un'email professionale, domani di aiutarmi a capire Heidegger, dopodomani di analizzare un problema tecnico complesso, e nel weekend di suggerirmi cosa cucinare con quello che ho in frigo. Claude risponde a tutto. Ma senza contesto, senza memoria del tuo profilo, senza sapere chi stai cercando di essere in quel momento, le risposte sono mediocri. Non perché Claude sia mediocre. Perché l'input è sbagliato.

Il vero problema, quello che ho impiegato un po' a formulare chiaramente, è che usiamo uno strumento potentissimo come se fosse un motore di ricerca glorificato. Fai una domanda, ottieni una risposta, chiudi la tab. E così sprechi quasi tutto il potenziale.

---

Da questa riflessione è nato quello che ho chiamato, con debito riconoscimento a De Bono, il sistema dei cappelli.

L'idea è banale nella forma, meno banale nell'esecuzione. Su Claude puoi creare dei Progetti, workspace separati con istruzioni persistenti. Ogni Progetto è un cappello. Ogni cappello ha un contesto preciso, un tono calibrato, regole specifiche, e accede solo ai dati rilevanti per quel momento.

Nel mio caso sono sei: il cappello del lavoro professionale, quello per l'esplorazione intellettuale, quello per i progetti creativi e la musica, quello per la vita personale e familiare, quello per il benessere fisico, quello per le finanze. Sei Claude diversi, ognuno con istruzioni su chi sono in quel momento, cosa mi serve, come voglio che mi risponda, cosa non deve fare.

La differenza pratica è quella che c'è tra parlare con qualcuno che ti conosce e qualcuno a cui devi sempre spiegare tutto da capo.

---

La connessione con De Bono non è solo nominale, ma non è nemmeno identica — e vale la pena dirlo.

Il principio profondo è lo stesso: separare i contesti mentali per non mescolarli. De Bono lo faceva per le riunioni di gruppo, per evitare che la critica uccidesse l'idea creativa prima che potesse respirare. Il sistema dei cappelli lo fa per la vita quotidiana, per evitare che il tono da professionista tecnico risponda quando stai cercando un interlocutore filosofico, o che le regole di compliance lavorative contaminino uno spazio in cui vuoi esplorare senza filtri.

Devo però essere preciso su una cosa: nel vocabolario di De Bono, il "pensiero laterale" e i "Sei Cappelli" sono due metodi distinti. Il pensiero laterale serve a generare idee nuove; i Sei Cappelli servono a esplorarle e svilupparle. Il titolo di questo articolo usa "separare i contesti" invece di "pensiero laterale" perché è quello che il sistema fa davvero — non è un'implementazione fedele del framework De Bono, è un'ispirazione che va in una direzione diversa.

C'è però una differenza sostanziale che un lettore attento avrebbe notata comunque. De Bono usava i cappelli come stati temporanei, maschere da indossare e togliere durante una sessione. Nel suo modello, il pericolo principale era trasformare i cappelli in tipi di personalità fissi, cosa che lui stesso metteva in guardia esplicitamente già nell'introduzione. Il sistema che ho costruito rischia esattamente questo: sei Progetti che diventano sei identità rigide invece di sei strumenti flessibili. È un limite reale, non un dettaglio. De Bono Ltd lo ha segnalato come uno degli errori più comuni nelle implementazioni AI del suo metodo — e il sistema dei cappelli che descrivo non ne è immune.

L'altra critica che un esperto del settore muoverebbe è tecnica: le istruzioni consumano token. Ogni parola che scrivi nelle istruzioni del Progetto è una parola in meno per il lavoro vero. Le istruzioni vanno tenute sotto le cinquecento parole, selezionando solo quello che cambia davvero il comportamento del modello. Scrivere un romanzo di contesto non ti dà un Claude più intelligente, ti dà conversazioni più corte.

E poi c'è il problema del context rot, che è il degrado progressivo della qualità quando le conversazioni diventano troppo lunghe. Il sistema dei cappelli non risolve questo problema, semplicemente lo sposta: invece di avere una chat caotica che accumula tutto, hai sei Progetti che accumulano conversazioni per contesto. La soluzione è aprire chat nuove spesso, non tenere una conversazione eterna dentro un Progetto.

---

Ho pubblicato tutto su GitHub.

La repo contiene le istruzioni complete per ognuno dei sei cappelli, i prompt template testati, e la struttura per generarne di nuovi in autonomia. Non è un prodotto, è un punto di partenza. Ogni persona ha contesti diversi, priorità diverse, modi di lavorare diversi. Il valore non è copiare quello che ho fatto io, è capire la logica e adattarla.

Il link è questo: [github.com/viciuslio/six-hats-claude](https://github.com/viciuslio/six-hats-claude)

---

Quello che ho imparato in questo processo, e che non mi aspettavo, è che la difficoltà non era tecnica.

Costruire le istruzioni dei Progetti è facile. La parte difficile è capire chi sei nei diversi contesti della tua vita. Cosa vuoi da un interlocutore quando stai lavorando a qualcosa di complesso e ad alto rischio. Cosa vuoi quando stai esplorando un'idea a cui tieni ma che non è ancora matura. Cosa vuoi quando hai bisogno di pensare a voce alta senza essere ottimizzato.

De Bono partiva dallo stesso punto. Il cappello non cambia come pensi, cambia come scegli di pensare. La distinzione è sottile ma fondamentale. Il cappello è uno strumento di intenzione, non di delega.

Forse il problema con l'AI, oggi, è proprio questo. Non sappiamo ancora cosa vogliamo, e la usiamo come se questo non importasse.

---

*Vicius Lio è Data & AI Engineer. Scrive di tecnologia, economia delle piattaforme e del rapporto tra innovazione digitale e società. Suona con Il Brigantino, esplorando la musica e la cultura popolare del Meridione d'Italia.*

---

**Fonti e riferimenti**

Edward De Bono, *Six Thinking Hats*, Little, Brown and Company, 1985.

Sul rapporto tra i Sei Cappelli e l'AI come strumento di prompting: Alan D. Thompson, *AI + Six Thinking Hats*, lifearchitect.ai, novembre 2023. Thompson usa il framework De Bono per visualizzare diverse prospettive sull'AI come fenomeno sociale — un uso diverso dal sistema descritto in questo articolo, ma che tocca la stessa metafora.

Sulla distinzione tra pensiero laterale e Sei Cappelli nel lavoro di De Bono: debono.com. Il pensiero laterale serve a creare idee; i Sei Cappelli servono a esplorarle e implementarle. Sono metodi complementari ma distinti.

Sul rischio di trattare i cappelli come tipi di personalità invece che come modalità temporanee: De Bono Ltd, six-thinking-hats.com. De Bono Ltd ha sviluppato sotto licenza una versione ufficiale del framework per ChatGPT, segnalando questo errore come uno dei più comuni nelle implementazioni non autorizzate.

Sulla gestione delle istruzioni nei Progetti Claude: J.D. Hodges, *Claude Custom Instructions: Real Examples and Best Practices*, jdhodges.com, febbraio 2026.

Sul context engineering come pratica emergente: *Claude best practices 2026: the complete power user guide*, The AI Corner, aprile 2026.
