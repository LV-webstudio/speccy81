# Idempotent geheugen (regel 11)

## Principes
- **Eén onderwerp per bestand** en een **korte index** (`GEHEUGEN.md`: één regel per bestand).
- **Toestandsbestanden** (wat verandert): **geheel herschreven** met «Toestand per <datum en tijd>», nooit met tekst
  achteraan toegevoegd. **Besluitbestanden** (wat stabiel is): niet aangeraakt tenzij het besluit verandert.
- **Een `hervatten.md`** als toegangspunt. Het wordt herschreven bij de afsluiting van elke fase of elk blok, en altijd vóór het
  opnieuw starten van een lange sessie (in plaats van te comprimeren).
- Koppelingen tussen bestanden met `[[naam]]`. Niets wat de repository al bewaart (code, git-geschiedenis).
- **Zonder geheimen of gegevens van derden.** De gegevens van de gebruiker zelf alleen in het lokale geheugen.
- **Alleen comprimeren bij het afsluiten van een blok**, met het geheugen al opgeslagen; als het vanzelf komt, wordt er hervat vanuit `hervatten.md`.

## Sjabloon `hervatten.md`
```markdown
---
name: hervatten
description: BEGIN HIER bij het openen van een nieuwe sessie over <project>: waar het werk is gebleven, open draden en wat eerst te controleren
metadata:
  type: project
---

**Toestand per <datum tijd>.** Idempotent bestand: geheel herschreven bij de afsluiting van elk blok.

## Wat eerst te controleren (5 minuten)
1. <laatste commit / schone werkmap>
2. <postvak of status van andere machines>
3. <actieve sessies en hun namen>

## Open draden (in volgorde)
| # | Draad | Volgende stap | Waar |
|---|---|---|---|

## Werkregels die niet veranderen
- <de onschendbare regels van het project>
```

## Sjabloon toestandsbestand
```markdown
---
name: <onderwerp>
description: <één regel om te beoordelen of het relevant is>
metadata:
  type: project
---

**Toestand per <datum tijd>.** Geheel herschreven.

- <feit> · <waar> · <openstaand> · <besluit dat op de gebruiker wacht>

Zie [[hervatten]].
```

## Index (`GEHEUGEN.md`)
```markdown
- [HERVATTEN · begin hier](hervatten.md) — waar het werk is gebleven en wat te controleren
- [<Onderwerp>](<onderwerp>.md) — <haakje van één regel>

Toestandsbestanden (…): ze worden GEHEEL HERSCHREVEN bij de afsluiting van elk blok. De rest zijn stabiele besluiten.
```
