# Incydent bezpieczeństwa (ujawniony klucz, dana lub kanał)

Otwiera się, gdy tylko pojawi się podejrzenie, bez czekania na pewność. W tym dokumencie bez sekretów i danych osobowych:
z kluczy tylko ich nazwa wewnętrzna i skrót; z osób tylko ich rola.

## Kroki
1. **Powstrzymać** to, co pilne: dezaktywować klucz, odciąć dostęp lub kanał. Jeśli to klucz, według zasady
   ujawnionego klucza: najpierw zastępczy; jeśli ujawnienie jest publiczne i pilne, dezaktywuje się go od razu, mówiąc
   wcześniej, co przestaje działać i dla kogo. Nigdy się go nie reaktywuje.
2. **Diagnozować tylko czytając:** co zostało ujawnione, od kiedy, gdzie i kto mógł to zobaczyć. Mierzy się (zasada 2):
   liczba, zapytanie lub polecenie, data.
3. **Zdecydować i zawiadomić:** decyduje użytkownik. Jeśli są dane osobowe klienta, klient jest **administratorem**,
   a Ty **podmiotem przetwarzającym**: zawiadamiasz go na piśmie **bez zbędnej zwłoki** (art. 33 ust. 2 RODO), z
   informacją, co się stało, od kiedy, co zrobiono i czego nie można wykluczyć. Administrator ocenia, czy zgłosić to organowi
   nadzorczemu ochrony danych w ciągu **72 godzin** (art. 33 RODO). Jeśli dane są Twoje, administratorem jesteś Ty.
4. **Zarejestrować** każdy incydent, nawet jeśli nie jest zgłaszany (art. 33 ust. 5 RODO): fakty, skutki i środki.
5. **Wniosek:** nowa zasada lub usprawnienie metody, które zapobiegnie powtórce.

## Karta
```markdown
# Incydent <n> · otwarty <data godzina> · stan: otwarty | powstrzymany | zamknięty
Co: <co zostało ujawnione, według nazwy wewnętrznej i skrótu; nigdy wartość>
Gdzie i od kiedy: <kanał, plik lub usługa · pierwsza możliwa data>
Kto mógł to zobaczyć: <publiczność | klienci | personel | nikt poza zespołem> — Dowód: <dziennik lub polecenie>
Powstrzymanie: <co dezaktywowano lub odcięto, kiedy> — Dowód: <…>
Co przestaje działać i dla kogo: <…>
Dane osobowe, których dotyczy: tak | nie | nie można wykluczyć — dlaczego
Administrator danych: <klient | my> · zawiadomienie wysłane?: <data, przez kogo> | szkic w <ścieżka>
Zgłoszenie do organu nadzorczego (decyduje administrator): tak | nie — powód
Środki: <…>
Wniosek: <nowa zasada lub usprawnienie>
```

## Przykład
Token API pojawia się w pliku konfiguracyjnym, który opublikowano w repozytorium. Powstrzymać: generuje się nowy token,
wstawia go wszędzie tam, gdzie jest używany, i odwołuje stary. Diagnozować: dziennik dostawcy mówi, czy ktoś użył tokenu i od kiedy.
Zarejestrować: karta wypełniona, nawet jeśli nie ma danych osobowych.
Wniosek: plik konfiguracyjny trafia do `.gitignore`, a repozytorium przegląda się przed publikacją.
