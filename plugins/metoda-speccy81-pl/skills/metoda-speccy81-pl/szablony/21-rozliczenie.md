# Rozliczenie (zasada 2)

Zamyka **każde** zlecenie, nawet krótkie. Trafia do użytkownika lub koordynatora (a z Wassup do wiadomości bezpośredniej
i do skrzynki). Jeśli brakuje któregokolwiek punktu, zlecenie pozostaje „nierozliczone”.

## Format
```markdown
## Rozliczenie · <zlecenie> · <data i godzina>
Polecenie (dosłownie): „<dokładny tekst polecenia, kto je wydał i w którym oknie>”
Zrobione:
- <co zrobiono, jedna linia na rzecz>
Dowód: <commit, skrót SHA-256, ścieżka, linia dziennika lub wynik polecenia>
Dowód: <po jednym na każdą zrobioną rzecz; może być z punktorem: „- Dowód: …”>
Niezrobione: <czego nie zrobiono> — <dlaczego (blokada uprawnień, brak danej, poza zakresem)>
Niesprawdzone: <co się twierdzi bez sprawdzenia> | nic
```

## Zasady
- Linia zaczyna się od `Dowód:` (lub `- Dowód:`). Etykieta według języka: es Prueba · en Proof · ca, pt i it Prova ·
  fr Preuve (ze spacją przed „:”) · de Nachweis · nl Bewijs · pl Dowód.
- Słowa **zrobione, sprawdzone, wysłane, wdrożone, usunięte, zainstalowane, opublikowane i zastosowane** bez
  `Dowód:` w tym samym punkcie są ostrzeżeniem.
- Dowód to coś, na co ktoś inny może spojrzeć jeszcze raz: „widziałem” nie jest dowodem; „zapisała to aplikacja” też nie,
  jeśli nie odczytano tego ponownie w miejscu docelowym.
- To, czego nie udało się dowieść, mówi się w „Niesprawdzone”, wraz z tym, kto ma to zrobić (np. „prawdziwy iPhone: czeka na
  urządzenie”).
- Jeśli później pojawi się błąd w czymś rozliczonym, **erratę** z tym samym nagłówkiem i „Poprawia: <data>”.

## Przykład
```markdown
## Rozliczenie · spis treści przewodnika · 01-03-2026 10:40
Polecenie (dosłownie): „Popraw zepsute odnośniki w spisie treści” (użytkownik, w oknie budowy)
Zrobione:
- 3 odnośniki poprawione w PRZEWODNIK.md
Dowód: commit 4f2a9c1
Dowód: `walidacja-wiedzy.sh` → „0 zepsutych odnośników”
Niezrobione: spis treści angielskiego README — nie należy do tej sesji (właściciel: przegląd)
Niesprawdzone: nic
```
