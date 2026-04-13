# Archivio LaTeX didattico

Repository per conservare, organizzare e versionare materiali didattici in **LaTeX** (verifiche, esercizi, programmazioni, relazioni e altri documenti) prodotti negli anni di insegnamento.

## Obiettivi

- Conservare i file in modo ordinato e ricercabile.
- Riutilizzare template e preamboli comuni.
- Tenere traccia delle revisioni tramite Git.
- Pubblicare materiali in formato aperto, pronti per essere aggiornati nel tempo.

## Struttura del repository

```text
.
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── INDEX.md
│   └── CONVENZIONI.md
├── templates/
│   ├── preamble.tex
│   └── verifica_template.tex
├── assets/
│   └── .gitkeep
├── fisica/
│   ├── biennio/
│   │   ├── esercizi/
│   │   └── verifiche/
│   └── triennio/
│       ├── esercizi/
│       └── verifiche/
├── matematica/
│   ├── biennio/
│   │   ├── esercizi/
│   │   └── verifiche/
│   └── triennio/
│       ├── esercizi/
│       └── verifiche/
└── altri-documenti/
    ├── comunicazioni/
    ├── programmazioni/
    └── relazioni/
```

## Convenzioni consigliate

- Nome file: `YYYY-MM-DD_materia_classe_tipo_argomento_vNN.tex`
- Esempio: `2024-10-21_fisica_3L_verifica_dinamica_v01.tex`
- Ogni documento dovrebbe contenere metadati iniziali (commenti) per facilitare ricerca e riuso.

Vedi i dettagli in: [`docs/CONVENZIONI.md`](docs/CONVENZIONI.md).

## Uso rapido

1. Copia il template da `templates/verifica_template.tex` nella cartella di destinazione.
2. Aggiorna titolo, classe, data e contenuti.
3. Compila con `latexmk -pdf nomefile.tex` (oppure il tuo flusso abituale).
4. Aggiorna l'indice in `docs/INDEX.md` se il documento è rilevante.

## Buone pratiche Git

- Commit piccoli e descrittivi.
- Evitare di versionare output compilati (`.pdf`) se non necessario.
- Usare branch dedicati solo per riorganizzazioni importanti.

## Privacy

Prima del push su GitHub:

- Rimuovere dati personali di studenti.
- Anonimizzare eventuali esempi di valutazione reali.
- Verificare eventuali allegati in `assets/`.

## Licenza

Il repository usa attualmente la licenza presente in `LICENSE`.
