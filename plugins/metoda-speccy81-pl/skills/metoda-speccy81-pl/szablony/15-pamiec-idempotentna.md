# Pamięć idempotentna (zasada 11)

## Zasady
- **Jeden temat na plik** i **krótki indeks** (`MEMORY.md`: jedna linia na plik).
- **Pliki stanu** (to, co się zmienia): **przepisywane w całości** ze stanem „Stan na <data i godzina>”, nigdy z tekstem
  dopisywanym na końcu. **Pliki decyzji** (to, co stałe): nie są ruszane, chyba że decyzja się zmieni.
- **Plik `wznowienie.md`** jako punkt wejścia. Jest przepisywany na zamknięcie każdej fazy lub bloku i zawsze przed
  restartem długiej sesji (zamiast kompaktowania).
- Odnośniki między plikami przez `[[nazwa]]`. Nic z tego, co już przechowuje repozytorium (kod, historia git).
- **Bez sekretów i danych osób trzecich.** Dane samego użytkownika tylko w pamięci lokalnej.
- **Kompaktowanie dopiero po zamknięciu bloku**, z już zapisaną pamięcią; jeśli nadejdzie samo, wznawia się od `wznowienie.md`.

## Szablon `wznowienie.md`
```markdown
---
name: wznowienie
description: ZACZNIJ TUTAJ, otwierając nową sesję w projekcie <projekt>: gdzie skończono, otwarte wątki i co sprawdzić w pierwszej kolejności
metadata:
  type: project
---

**Stan na <data godzina>.** Plik idempotentny: przepisywany w całości na zamknięcie każdego bloku.

## Co sprawdzić w pierwszej kolejności (5 minut)
1. <ostatni commit / czyste drzewo>
2. <skrzynka lub stan pozostałych komputerów>
3. <aktywne sesje i ich nazwy>

## Otwarte wątki (w kolejności)
| # | Wątek | Następny krok | Gdzie |
|---|---|---|---|

## Zasady pracy, które się nie zmieniają
- <nienaruszalne zasady projektu>
```

## Szablon pliku stanu
```markdown
---
name: <temat>
description: <jedna linia, by ocenić, czy jest istotny>
metadata:
  type: project
---

**Stan na <data godzina>.** Przepisany w całości.

- <fakt> · <gdzie> · <zaległe> · <decyzja oczekująca na użytkownika>

Zobacz [[wznowienie]].
```

## Indeks (`MEMORY.md`)
```markdown
- [WZNOWIENIE · zacznij tutaj](wznowienie.md) — gdzie skończono pracę i co sprawdzić
- [<Temat>](<temat>.md) — <hasło w jednej linii>

Pliki stanu (…): są PRZEPISYWANE w całości na zamknięcie każdego bloku. Pozostałe to decyzje stałe.
```
