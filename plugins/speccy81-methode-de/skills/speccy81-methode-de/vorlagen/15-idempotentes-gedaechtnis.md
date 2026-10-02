# Idempotentes Gedächtnis (Regel 11)

## Prinzipien
- **Ein Thema pro Datei** und ein **kurzer Index** (`MEMORY.md`: eine Zeile pro Datei).
- **Statusdateien** (was sich ändert): werden **vollständig neu geschrieben** mit «Stand: <Datum und Uhrzeit>», nie wird
  Text am Ende angehängt. **Entscheidungsdateien** (was stabil ist): werden nicht angefasst, außer die Entscheidung ändert sich.
- **Eine `fortsetzen.md`** als Einstiegspunkt. Sie wird beim Abschluss jeder Phase oder jedes Blocks neu geschrieben und immer, bevor
  eine lange Sitzung neu gestartet wird (statt zu komprimieren).
- Verweise zwischen Dateien mit `[[name]]`. Nichts, was das Repository bereits festhält (Code, Git-Historie).
- **Keine Geheimnisse oder Daten Dritter.** Die Daten des Nutzers selbst nur im lokalen Gedächtnis.
- **Nur beim Abschluss eines Blocks komprimieren**, mit bereits gespeichertem Gedächtnis; kommt es von selbst, wird von `fortsetzen.md` aus weitergemacht.

## Vorlage für `fortsetzen.md`
```markdown
---
name: fortsetzen
description: HIER BEGINNEN beim Öffnen einer neuen Sitzung zu <Projekt>: wo es stehen geblieben ist, offene Fäden und was zuerst zu prüfen ist
metadata:
  type: project
---

**Stand: <Datum Uhrzeit>.** Idempotente Datei: wird beim Abschluss jedes Blocks vollständig neu geschrieben.

## Was zuerst zu prüfen ist (5 Minuten)
1. <letzter Commit / sauberer Arbeitsbaum>
2. <Postfach oder Status anderer Rechner>
3. <aktive Sitzungen und ihre Namen>

## Offene Fäden (der Reihe nach)
| # | Faden | Nächster Schritt | Wo |
|---|---|---|---|

## Arbeitsregeln, die sich nicht ändern
- <die unverletzlichen Regeln des Projekts>
```

## Vorlage für eine Statusdatei
```markdown
---
name: <thema>
description: <eine Zeile, um zu entscheiden, ob sie relevant ist>
metadata:
  type: project
---

**Stand: <Datum Uhrzeit>.** Wird vollständig neu geschrieben.

- <Fakt> · <wo> · <offen> · <Entscheidung, die auf den Nutzer wartet>

Siehe [[fortsetzen]].
```

## Index (`MEMORY.md`)
```markdown
- [FORTSETZEN · hier beginnen](fortsetzen.md) — wo die Arbeit stehen geblieben ist und was zu prüfen ist
- [<Thema>](<thema>.md) — <Aufhänger in einer Zeile>

Statusdateien (…): werden beim Abschluss jedes Blocks vollständig NEU GESCHRIEBEN. Die übrigen sind stabile Entscheidungen.
```
