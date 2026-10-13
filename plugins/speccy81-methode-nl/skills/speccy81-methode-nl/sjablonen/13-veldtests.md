# Veldtests · <project> · <datum>

## 1. Opzet (controleer VÓÓR het begin)
| Wat | Waarde | Gecontroleerd? |
|---|---|---|
| Machines en apparaten (model, besturingssysteem, appversie) | | |
| Hoe elk onderdeel wordt gestart (**vanuit een schone terminal**, niet vanuit een andere sessie of ander proces dat variabelen overerft) | | |
| Toestemmingsmodus / configuratie van elke sessie (bijv. geen automatische modus als goedkeuringen worden getest) | | |
| Instellingen die de test aan moet hebben staan (bijv. pushmeldingen, Remote Control, USB-foutopsporing) | | |
| Testgegevens (echt of seed; nooit persoonsgegevens in schermafbeeldingen die worden bewaard) | | |
| Wie uitvoert en wie observeert (gebruiker / sessie / andere machine) | | |
| Hoe wordt geobserveerd (schermafbeeldingen, ADB, logs, `dumpsys`, console) | | |
| **Poort «compileert»:** typecontrole en productiebuild groen op de commit die wordt getest (de ontwikkelserver garandeert dat niet) | | |

## 2. Tests
| # | Test | Wat het bevestigt | Stappen | Verwacht resultaat | Prioriteit |
|---|---|---|---|---|---|
| P1 | | | | | Hoog |

## 3. Resultaten
| # | Resultaat (✅ / ❌ / ⚠ ongeldig) | Tijd | Bewijs (schermafbeelding, uitvoer) | Detail |
|---|---|---|---|---|
| P1 | | | | |

«⚠ ongeldig» = de opzet voldeed niet aan tabel 1; de test wordt herhaald en telt niet als productfout.

**Een mislukte test wordt niet overgeslagen:** hij wordt herhaald (bijv. 3 keer) om te weten of hij instabiel of echt is, de schermafbeelding wordt bekeken en er wordt uitgezocht of de test of de app faalt. Wordt hij uiteindelijk toch overgeslagen, dan staat hij als «overgeslagen» en met de reden.

## 4. Bevindingen en wijzigingen
| Bevinding | Raakt (regel / document / code) | In dezelfde stap aangebrachte wijziging |
|---|---|---|
| | | |

## 5. Nog te herhalen
-
