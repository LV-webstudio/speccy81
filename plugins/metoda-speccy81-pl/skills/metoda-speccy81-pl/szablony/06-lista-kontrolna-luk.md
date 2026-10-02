# Analiza luk · „czego brakuje, żeby zrobić to jakościowo?”

Pytanie przewodnie: *co decyduje o jakości końcowego wyniku, który widzi klient, i czy jest to pokryte
konkretnymi danymi, które silnik może zastosować?*

Dla każdego tematu: przeszukaj `wiedza/` (grep po kluczowych terminach) i zaznacz.

| Temat | Terminy do wyszukania | Dokumenty, które to pokrywają | Wystarczy do obliczeń? | Działanie |
|---|---|---|---|---|
| Jak krok po kroku wykonuje się pracę (technika) | | | | |
| Parametry liczbowe (prędkości, czasy, rozmiary, marginesy) | | | | |
| Co można, a czego nie można kontrolować w narzędziach/sprzęcie | | | | |
| Symulacja lub walidacja przed wykonaniem naprawdę | | | | |
| Warunki zewnętrzne (pogoda, światło, pora dnia, pora roku) | | | | |
| Bezpieczeństwo, sytuacje awaryjne i incydenty | | | | |
| Przypadki graniczne (trudne środowiska, awarie) | | | | |
| Przetwarzanie końcowe i dostawa (formaty, kontrola jakości) | | | | |
| Automatyzacja przetwarzania końcowego | | | | |
| Prawdziwe przykłady (pliki, próbki) | | | | |
| Szkolenie zespołu | | | | |
| Szczególne ryzyka pracownicze i prawne | | | | |
| **Testy na prawdziwych danych lub w prawdziwym użyciu** (czy jest minimalne stanowisko testowe? czy już próbowano?) | | | | |
| **Prywatność i minimalizacja danych** (co jest odczytywane, przechowywane i wysyłane; RODO) | | | | |
| **Wdrożenie i istniejące systemy** (gdzie działa, z czym się łączy, co się stanie po przeniesieniu) | | | | |

Tylko rzeczywiste luki uruchamiają nowy blok badań. Powtarzaj, aż nie zostaną żadne istotne luki.
Wszystko, co zależy od warunków (pogoda, światło, dane klienta), musi trafić do **selektora**
z regułami, a nie do luźnego tekstu.
