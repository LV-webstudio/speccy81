# Memoria idempotente (regola 11)

## Principi
- **Un argomento per file** e un **indice breve** (`MEMORY.md`: una riga per file).
- **File di stato** (ciò che cambia): **riscritti per intero** con «Stato al <data e ora>», mai con testo
  aggiunto in fondo. **File di decisione** (ciò che è stabile): non si toccano a meno che la decisione non cambi.
- **Un `riprendi.md`** come punto di ingresso. Si riscrive alla chiusura di ogni fase o blocco, e sempre prima di
  riavviare una sessione lunga (invece di compattare).
- Collegamenti tra file con `[[nome]]`. Niente di ciò che il repository conserva già (codice, cronologia git).
- **Niente segreti né dati di terzi.** I dati dell'utente stesso, solo nella memoria locale.
- **Compattare solo alla chiusura di un blocco**, con la memoria già salvata; se arriva da sola, si riprende da `riprendi.md`.

## Modello di `riprendi.md`
```markdown
---
name: riprendi
description: INIZIA DA QUI quando apri una nuova sessione su <progetto>: dove si era rimasti, fili aperti e cosa controllare per primo
metadata:
  type: project
---

**Stato al <data ora>.** File idempotente: si riscrive per intero alla chiusura di ogni blocco.

## Cosa controllare per primo (5 minuti)
1. <ultimo commit / albero pulito>
2. <casella di posta o stato delle altre macchine>
3. <sessioni attive e i loro nomi>

## Fili aperti (in ordine)
| # | Filo | Passo successivo | Dove |
|---|---|---|---|

## Regole di lavoro che non cambiano
- <le regole inviolabili del progetto>
```

## Modello di file di stato
```markdown
---
name: <argomento>
description: <una riga per decidere se è pertinente>
metadata:
  type: project
---

**Stato al <data ora>.** Riscritto per intero.

- <fatto> · <dove> · <in sospeso> · <decisione in attesa dell'utente>

Vedi [[riprendi]].
```

## Indice (`MEMORY.md`)
```markdown
- [RIPRENDI · inizia da qui](riprendi.md) — dove si è interrotto il lavoro e cosa controllare
- [<Argomento>](<argomento>.md) — <aggancio di una riga>

File di stato (…): si RISCRIVONO per intero alla chiusura di ogni blocco. Gli altri sono decisioni stabili.
```
