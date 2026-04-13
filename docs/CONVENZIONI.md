# Convenzioni di organizzazione

## 1) Nomenclatura dei file

Formato consigliato:

`YYYY-MM-DD_materia_classe_tipo_argomento_vNN.tex`

Dove:
- `YYYY-MM-DD`: data di creazione/somministrazione.
- `materia`: `fisica`, `matematica`, ecc.
- `classe`: es. `2B`, `3L`, `5A`.
- `tipo`: `verifica`, `esercizi`, `simulazione`, `relazione`, `programmazione`.
- `argomento`: parole in minuscolo separate da trattino.
- `vNN`: versione a due cifre (`v01`, `v02`, ...).

Esempio:

`2025-02-10_matematica_4A_verifica_funzioni-goniometriche_v03.tex`

## 2) Metadati nel file `.tex`

Inserire all'inizio del documento:

```tex
% materia: Matematica
% classe: 4A
% tipo: Verifica
% anno_scolastico: 2025-2026
% argomenti: funzioni goniometriche
% versione: 03
```

## 3) Organizzazione per cartelle

- **Materia**: `fisica/`, `matematica/`, ...
- **Livello**: `biennio/`, `triennio/`
- **Tipo**: `verifiche/`, `esercizi/`
- **Altri documenti**: `altri-documenti/`

## 4) Versionamento

- Incrementare `vNN` per modifiche sostanziali.
- Preferire commit frequenti con messaggi chiari.
- Evitare commit con decine di file non correlati.

## 5) PDF e output compilati

Per default gli output temporanei LaTeX sono ignorati da `.gitignore`.
Versionare i PDF finali solo se necessario per distribuzione.
