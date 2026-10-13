# Feldtests · <Projekt> · <Datum>

## 1. Aufbau (VOR dem Start prüfen)
| Was | Wert | Geprüft? |
|---|---|---|
| Rechner und Geräte (Modell, Betriebssystem, App-Version) | | |
| Wie jedes Teil gestartet wird (**aus einem sauberen Terminal**, nicht aus einer anderen Sitzung oder einem Prozess, der Variablen vererbt) | | |
| Berechtigungsmodus / Konfiguration jeder Sitzung (z. B. kein automatischer Modus, wenn Freigaben getestet werden) | | |
| Einstellungen, die der Test eingeschaltet braucht (z. B. Push-Benachrichtigungen, Remote Control, USB-Debugging) | | |
| Testdaten (echt oder Seed; nie personenbezogene Daten auf gespeicherten Screenshots) | | |
| Wer ausführt und wer beobachtet (Nutzer / Sitzung / anderer Rechner) | | |
| Wie beobachtet wird (Screenshots, ADB, Logs, `dumpsys`, Konsole) | | |
| **Tor «kompiliert»:** Typprüfung und Produktions-Build grün auf dem getesteten Commit (der Entwicklungsserver garantiert das nicht) | | |

## 2. Tests
| # | Test | Was er bestätigt | Schritte | Erwartetes Ergebnis | Priorität |
|---|---|---|---|---|---|
| P1 | | | | | Hoch |

## 3. Ergebnisse
| # | Ergebnis (✅ / ❌ / ⚠ ungültig) | Zeit | Beleg (Screenshot, Ausgabe) | Detail |
|---|---|---|---|---|
| P1 | | | | |

«⚠ ungültig» = der Aufbau erfüllte Tabelle 1 nicht; der Test wird wiederholt und zählt nicht als Produktfehler.

**Ein fehlschlagender Test wird nicht übersprungen:** Er wird wiederholt (z. B. 3-mal), um zu wissen, ob er instabil oder echt ist, der Screenshot wird angesehen und geklärt, ob der Test oder die App fehlschlägt. Wird er am Ende doch übersprungen, steht er als «übersprungen» und mit dem Grund da.

## 4. Erkenntnisse und Änderungen
| Erkenntnis | Betrifft (Regel / Dokument / Code) | Gleichzeitig vorgenommene Änderung |
|---|---|---|
| | | |

## 5. Noch zu wiederholen
-
