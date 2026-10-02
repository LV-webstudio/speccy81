# Metodo Speccy81

![Speccy81 Method](assets/banner.jpg)

**Dall'idea al lancio.** Un metodo di LV-Webstudio (Speccy81) per impostare qualsiasi progetto — prodotto, servizio, modulo o app — con lo stesso rigore: prima la ricerca, decidere con i dati, trasformare ciò che impari in conoscenza verificata, sottoporla ad audit, progettare prima di programmare, provare sul campo e pubblicare senza sorprese. Ha due edizioni costruite dallo stesso metodo, ciascuna come marketplace di plugin per Claude Code.

Questa è l'**edizione base**: libera e pubblica, con una skill, una guida breve e 8 modelli in ogni lingua.

**Languages · Idiomas:** [English](README.md) · [Español](README.es.md) · [Català](README.ca.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Português](README.pt.md) · [Français](README.fr.md) · [Italiano](README.it.md) · [Deutsch](README.de.md)

## Edizioni

| | Base | Completa |
|---|---|---|
| Licenza | Pubblica: CC BY 4.0 (guida, SKILL e modelli) + MIT (script); vedi `NOTICE` | Proprietaria, di LV-Webstudio |
| Percorso | Un percorso leggero in cinque passi per ampliamenti e piccoli progetti | Fasi 0–9 più la 8 bis |
| Modelli | 8 (01, 06, 09, 10, 13, 15, 20 e 21) | 24 |
| Regole d'oro | Le 13, in forma breve, e le 10 regole brevi del team | Le 13 per intero, le 10 regole brevi del team con i loro allegati e i miglioramenti di efficienza E1–E15 |
| Ricerca e audit | — | Ondate di ricerca in parallelo e un audit unico |
| Validatore della conoscenza | — | Sì |
| Rilascio e lancio | — | Rilascio e QA su un altro dispositivo, e pubblicazione |
| Governo e sicurezza | Regola 13 in forma breve, «Prova:» in ogni risultato, incidenti (20) e rendiconto (21) | In più: governo di più team (19), trasferire un segreto, ruotare una chiave esposta, migrazione dei dati (22), passaggio di consegne o cambio di macchina (23) e checklist della privacy (24) |
| Più macchine | Una sola sessione o macchina; per più sessioni con regole minime, Wassup Base | Governo completo e coordinamento facoltativo con Wassup |

## I cinque passi

| Passo | Cosa succede | Modello |
|---|---|---|
| 1 · Fase 0 | Scheda di contesto; se il progetto è già avviato, vi si raccoglie ciò che esiste (codice, documenti, decisioni) | 01 |
| 2 | Checklist delle lacune e fatti canonici, prima di ricercare o progettare | 06, 10 |
| 3 · Fase 7 | Progetto breve, approvato dall'utente prima di programmare | 09 |
| 4 · Fase 8 | Costruzione con prove reali e sul campo | 13 |
| 5 | Memoria idempotente alla chiusura di ogni passo | 15 |
| Sempre | Rendiconto con «Prova:» alla chiusura di ogni incarico; incidente se si espone una chiave o un dato | 21, 20 |

La numerazione delle fasi (0, 7 e 8) è quella del metodo completo, così il progetto può crescere senza rinumerare nulla. L'edizione completa aggiunge il resto: le fasi da 1 a 6, la 8 bis e la 9.

## Cosa contiene

Un plugin per lingua, ciascuno con la skill, la guida e gli 8 modelli: `speccy81-method` (English), `metodo-speccy81` (Español), `metode-speccy81-ca` (Català), `metodo-speccy81-pt` (Português), `methode-speccy81-fr` (Français), `metodo-speccy81-it` (Italiano), `speccy81-methode-de` (Deutsch), `speccy81-methode-nl` (Nederlands) e `metoda-speccy81-pl` (Polski).

Tutti i plugin contengono lo stesso metodo; installa quello nella lingua che preferisci.

## Installazione

```
claude plugin marketplace add LV-webstudio/speccy81
claude plugin install speccy81-method@speccy81      # English
claude plugin install metodo-speccy81@speccy81      # Español
claude plugin install metode-speccy81-ca@speccy81   # Català
claude plugin install metodo-speccy81-pt@speccy81   # Português
claude plugin install methode-speccy81-fr@speccy81  # Français
claude plugin install metodo-speccy81-it@speccy81   # Italiano
claude plugin install speccy81-methode-de@speccy81  # Deutsch
claude plugin install speccy81-methode-nl@speccy81  # Nederlands
claude plugin install metoda-speccy81-pl@speccy81   # Polski
```

Poi chiedi a Claude Code di «applicare il metodo Speccy81», anche per un progetto già avviato. La skill carica la guida e i modelli quando servono.

[Wassup](https://github.com/LV-webstudio/wassup) è un complemento facoltativo quando più macchine o sessioni lavorano sullo stesso progetto.

## Come ottenere l'edizione completa

L'edizione completa è concessa in licenza da LV-Webstudio. Richiedi l'accesso tramite [lv-webstudio.com](https://lv-webstudio.com/).

## Licenza

L'edizione base è offerta con due licenze: **CC BY 4.0** per la guida, SKILL.md e i modelli (uso libero, anche commerciale, con attribuzione) e **MIT** per script e codice. Attribuzione suggerita: «Método Speccy81 · LV-Webstudio · lv-webstudio.com». L'edizione completa non è coperta da queste licenze. Vedi [LICENSE](LICENSE).
