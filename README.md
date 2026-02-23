Nome del progetto
Visualizzare la Controriforma: analisi dei soggetti e delle funzioni artistiche prima e dopo il 1563

DOI

DOI del record su Zenodo

Descrizione
Questo progetto analizza l’evoluzione dei soggetti e della funzione delle opere d’arte europee tra il 1400 e il 1700, con particolare attenzione al periodo successivo al Concilio di Trento (1563).
L’analisi è stata realizzata utilizzando metadati delle opere del MET e implementata in un notebook Python su Google Colab.

In cosa consiste il progetto?
Il progetto consiste dei seguenti obbiettivi:
- Analizzare la variazione della proporzione tra soggetti religiosi e mitologici
- Analizzare la funzione delle opere (religiosa vs decorativa/classica)
- Analizzare i soggetti religiosi più rappresentati pre/post Concilio


Quali sono i risultati?
L’analisi non evidenzia un aumento quantitativo delle opere religiose dopo il Concilio di Trento (1563). La produzione religiosa rimane prevalente rispetto a quella mitologica in entrambi i periodi, ma la sua proporzione diminuisce nel periodo 1563–1700. I dati suggeriscono quindi una continuità della centralità del tema religioso, senza un incremento significativo post-1563.

Fonte dei dati

Descrizione dei dati
I dati utilizzati in questo progetto provengono dalla Open Access Collection del Metropolitan Museum of Art (MET). La banca dati del MET contiene metadati descrittivi di oltre 470.000 opere d’arte, tra cui informazioni su titolo, artista, data di creazione, genere, contenuti e soggetti. Questi dati sono stati distribuiti in formato CSV e sono liberamente accessibili per uso di ricerca, analisi e visualizzazione.

Citazione e link alle fonti dei dati utilizzati
I dati sono stati scaricati dalla repository ufficiale dell’iniziativa Open Access del MET:
Open Access del MET (dati e immagini): https://www.metmuseum.org/es/hubs/open-access
Repository ufficiale con dataset CSV: https://github.com/metmuseum/openaccess

Metodi e strumenti
L’analisi è stata realizzata in ambiente Python utilizzando Google Colab.
Il dataset è stato importato in formato CSV e manipolato tramite la libreria Pandas. In una prima fase è stato filtrato l’intervallo cronologico 1400–1700 utilizzando condizioni logiche sulla variabile `data_creazione`. Successivamente il campione è stato suddiviso in due sottoinsiemi (1400–1563 e 1563–1700) attraverso operazioni di pulizia del DataFrame.
Sono state poi create nuove variabili categoriali (es. `categoria_soggetto`, `categoria_funzione`) tramite funzioni di classificazione applicate ai metadati testuali (titoli e descrizioni).
Per l’analisi quantitativa sono state utilizzate:
`value_counts()` e `value_counts(normalize=True)` 

Strumenti utilizzati:
Python
Google Colab
Pandas (manipolazione e analisi dati)
Matplotlib (visualizzazione grafica)
Dataset Open Access del Metropolitan Museum of Art (CC0)


Responsabili

Di Pane, Ramona - ORCID 0009-0008-8880-2572 
Landi, Lucia - ORCID 0009-0001-8380-3356 

Licenza

Nome e link alla licenza
