# Rechenschaft (Regel 2)

Schließt **jeden** Auftrag ab, auch einen kurzen. Geht an den Nutzer oder an den Koordinator (und, mit Wassup, an den direkten Kanal und an das
Postfach). Fehlt ein Abschnitt, bleibt der Auftrag «ohne Rechenschaft».

## Format
```markdown
## Rechenschaft · <Auftrag> · <Datum und Uhrzeit>
Befehl (wörtlich): «<genauer Text des Befehls, mit Angabe, von wem er kam und in welchem Fenster>»
Erledigt:
- <was getan wurde, eine Zeile pro Sache>
Nachweis: <Commit, SHA-256-Hash, Pfad, Protokollzeile oder Ausgabe eines Befehls>
Nachweis: <einer pro erledigter Sache; gilt auch mit Aufzählungszeichen: «- Nachweis: …»>
Nicht erledigt: <was nicht getan wurde> — <warum (Berechtigungssperre, fehlende Angabe, außerhalb des Umfangs)>
Ungeprüft: <was ohne Prüfung behauptet wird> | nichts
```

## Regeln
- Die Zeile beginnt mit `Nachweis:` (oder `- Nachweis:`). Label je Sprache: es Prueba · en Proof · ca, pt und it Prova ·
  fr Preuve (mit Leerzeichen vor «:») · de Nachweis · nl Bewijs · pl Dowód.
- Die Wörter **erledigt, geprüft, hochgeladen, deployt, gelöscht, installiert, veröffentlicht und angewendet** ohne einen
  `Nachweis:` im selben Abschnitt sind eine Warnung.
- Ein Nachweis ist etwas, das ein anderer erneut ansehen kann: «ich habe es gesehen» ist kein Nachweis; «die App hat es gespeichert» ebenfalls nicht, wenn
  es nicht am Ziel erneut gelesen wurde.
- Was sich nicht nachweisen ließ, wird unter «Ungeprüft» gesagt, mit der Angabe, wer es tun muss (z. B. «echtes iPhone: Gerät
  ausstehend»).
- Taucht später ein Fehler in etwas bereits Rechenschaftspflichtigem auf, folgt eine **Berichtigung** mit derselben Kopfzeile und «Korrigiert: <Datum>».

## Beispiel
```markdown
## Rechenschaft · Index des Leitfadens · 01.03.2026 10:40
Befehl (wörtlich): «Korrigiere die defekten Links des Index» (Nutzer, im Fenster des Aufbaus)
Erledigt:
- 3 Links in LEITFADEN.md korrigiert
Nachweis: Commit 4f2a9c1
Nachweis: `wissen-validieren.sh` → «0 defekte Links»
Nicht erledigt: der Index der englischen README — gehört nicht zu dieser Sitzung (Eigentümer: Prüfung)
Ungeprüft: nichts
```
