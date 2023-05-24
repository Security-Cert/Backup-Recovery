Questo sarà il primo di una serie di articoli in cui parlerò di backup & Disaster Recovery, elementi fondamentali per preservare le informazioni digitali da eventuali incidenti.

# Il backup:
Il **backup** in informatica indica la messa in sicurezza delle **informazioni** di un sistema informatico attraverso la creazione di **ridondanza** delle informazioni stesse (una o più copie di riserva dei dati), da utilizzare come recupero (ripristino) dei dati stessi in caso di eventi malevoli accidentali o intenzionali o semplice manutenzione del sistema. 
[[backup - Wikipedia](https://it.wikipedia.org/wiki/Backup)]

Il backup è una misura di sicurezza **fondamentale** che non deve essere sottovalutata, perchè nella maggior parte dei casi è l'unica soluzione per recuperare i dati dopo un incidente informatico.
Anche se si mettono in atto tutte le misure di prevenzione, un incidente che compromette i dati può sempre accadere, **il rischio 0 non esiste.**

# Il Disaster Recovery Plan:
Il backup è una misura che fa parte del **Disaster Recovery Plan (DRP)**, il piano che ogni azienda dovrebbe aver predisposto per essere pronta ad affrontare qualsiasi tipo di incidente informatico.
Questo documento include istruzioni dettagliate su come **rispondere** a incidenti non pianificati come disastri naturali, interruzioni di corrente, attacchi informatici e qualsiasi altra interruzione. Il piano comprende le strategie per ridurre al minimo gli effetti di un incidente, in modo che un'organizzazione continui ad operare o riprenda rapidamente le operazioni principali.

La valutazione del rischio e un'analisi dell'impatto aziendale che quantifichi i possibili effetti di un evento disastroso sono strumenti efficaci per ottenere assistenza nella gestione di un piano di Disaster Recovery.

# Analisi - RPO,RTO e SLO:
Alla base di tutto ci deve essere un'analisi, che parte da queste semplici domande:

1. Quanto sono imporatnti i miei dati?
2. Quanti dati posso permettermi di perdere senza creare un danno alla mia azienda?
3. Quanto tempo posso perdere per il ripristino dei miei dati, prima di subire danni?

Dalle risposte a queste domande si arriva ad ottenere:

* **Il Recovery Point Objective (RPO):** Rappresenta il massimo tempo entro il quale deve essere fatto il backup di un dato. Ci indica la misura della quantità di dati che siamo disposti a perdere a casusa di un incidente. E', in pratica, l'intervallo di tempo che intercorre tra un backup e quello successivo. Da RPO dipende la scelta della **frequenza** temporale di backup;
* **Il Recovery Time Objective (RTO):** E' il tempo entro il quale l'azienda deve essere in grado di ripristinare la sua operatività. In pratica il tempo massimo che si ritiene **tollerabile** per un downtime (blocco dell'operatività);
* **Service Level Objective (SLO):** Rappresenta la somma dei tempi RPO + RTO.

Nell'immagine seguente, vediamo cosa rappresentano in una scala temporale RPO e RTO rispetto al momento dell'evento critico.

![Cosa sono RPO e RTO](https://imgcdn.agendadigitale.eu/wp-content/uploads/2019/03/07081302/image_0.png)

Una volta fatta quest'analisi possiamo stabilire:

* Quali dati inserire nei backup;
* La frequenza con cui fare i backup (un'ora, un giorno, un mese, ecc.);
* La modalità con cui fare i backup (NAS, cloud, nastri, ecc.).

Tutto questo andrà fatto sulla base di una valutazione **costi/benefici**, perchè una riduzione dei tempi di RPO e RTO riduce i tempi di fermo dell'azienda, ma aumenta i costi di backup.

# Conclusione:
Come primo articolo abbiamo parlato di cosa sono, soprattutto di quanto siano importanti, i backup e il Disaster Recovery Plan.
Nelle prossime uscite approfondiremo questi argomenti in modo più dettagliato, partendo dalla loro storia.


**Riferimenti:**

[[Immagine - Cosa sono RPO e RTO | agendadigitale.eu ](https://www.agendadigitale.eu/infrastrutture/business-continuity-e-disaster-recovery-ecco-le-strategie-a-prova-di-emergenza/)]

[[L'importanza dei backup | giorgiosbaraglia.it ](https://www.giorgiosbaraglia.it/pubblicata-la-2a-edizione-del-libro-cyber-security-kit-di-sopravvivenza/)]