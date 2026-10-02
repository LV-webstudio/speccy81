# Rekenschap (regel 2)

Sluit **elke** opdracht af, ook een korte. Gaat naar de gebruiker of de coördinator (en, met Wassup, naar het directe bericht en het
postvak). Als een onderdeel ontbreekt, blijft de opdracht «zonder rekenschap».

## Formaat
```markdown
## Rekenschap · <opdracht> · <datum en tijd>
Instructie (letterlijk): «<exacte tekst van de instructie, met wie ze gaf en in welk venster>»
Gedaan:
- <wat is gedaan, één regel per ding>
Bewijs: <commit, SHA-256-hash, pad, logregel of uitvoer van een opdracht>
Bewijs: <één per gedaan ding; mag met opsommingsteken: «- Bewijs: …»>
Niet gedaan: <wat niet is gedaan> — <waarom (toestemmingen geblokkeerd, een gegeven ontbreekt, buiten bereik)>
Zonder controle: <wat wordt beweerd zonder het te hebben gecontroleerd> | niets
```

## Regels
- De regel begint met `Bewijs:` (of `- Bewijs:`). Label per taal: es Prueba · en Proof · ca, pt en it Prova ·
  fr Preuve (met een spatie vóór «:») · de Nachweis · nl Bewijs · pl Dowód.
- De woorden **gedaan, gecontroleerd, geüpload, uitgerold, verwijderd, geïnstalleerd, gepubliceerd en toegepast** zonder een
  `Bewijs:` in hetzelfde onderdeel zijn een waarschuwing.
- Een bewijs is iets wat een ander opnieuw kan bekijken: «ik heb het gezien» is geen bewijs; «de app heeft het opgeslagen» ook niet, als het niet
  op de bestemming is teruggelezen.
- Wat niet kon worden bewezen, wordt gezegd bij «Zonder controle», met wie het moet doen (bijv. «echte iPhone: wacht op
  apparaat»).
- Als er achteraf een fout blijkt in iets wat is verantwoord, volgt een **erratum** met dezelfde kop en «Corrigeert: <datum>».

## Voorbeeld
```markdown
## Rekenschap · index van de gids · 01-03-2026 10:40
Instructie (letterlijk): «Corrigeer de kapotte links van de index» (gebruiker, in het bouwvenster)
Gedaan:
- 3 links gecorrigeerd in GIDS.md
Bewijs: commit 4f2a9c1
Bewijs: `kennis-valideren.sh` → «0 kapotte links»
Niet gedaan: de index van de Engelse README — niet van deze sessie (eigenaar: review)
Zonder controle: niets
```
