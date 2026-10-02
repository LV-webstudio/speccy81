# Sicherheitsvorfall (offengelegter Schlüssel, offengelegte Daten oder offengelegter Kanal)

Wird eröffnet, sobald ein Verdacht besteht, ohne zu warten, bis man sicher ist. Keine Geheimnisse oder personenbezogenen Daten in diesem Dokument:
von Schlüsseln nur der interne Name und der Hash; von Personen nur ihre Rolle.

## Schritte
1. **Eindämmen**, was dringend ist: den Schlüssel deaktivieren, den Zugang oder den Kanal kappen. Handelt es sich um einen Schlüssel, nach der Regel des
   offengelegten Schlüssels: zuerst der Ersatz; ist die Offenlegung öffentlich und dringend, wird er sofort deaktiviert, wobei vorher gesagt wird, was nicht mehr
   funktioniert und für wen. Er wird nie reaktiviert.
2. **Nur lesend diagnostizieren:** was offengelegt wurde, seit wann, wo und wer es sehen konnte. Es wird gemessen (Regel 2):
   Zahl, Abfrage oder Befehl, Datum.
3. **Entscheiden und benachrichtigen:** Der Nutzer entscheidet. Liegen personenbezogene Daten eines Kunden vor, ist der Kunde der **Verantwortliche**
   und Sie der **Auftragsverarbeiter**: Sie benachrichtigen ihn schriftlich **unverzüglich** (Art. 33 Abs. 2 DSGVO) darüber, was geschehen ist, seit
   wann, was getan wurde und was sich nicht ausschließen lässt. Der Verantwortliche prüft, ob er die Datenschutzaufsichtsbehörde
   innerhalb von **72 Stunden** benachrichtigt (Art. 33). Sind es Ihre eigenen Daten, sind Sie der Verantwortliche.
4. **Dokumentieren** jeden Vorfalls, auch wenn er nicht gemeldet wird (Art. 33 Abs. 5): Tatsachen, Auswirkungen und Maßnahmen.
5. **Lehre:** die neue Regel oder die Verbesserung der Methode, die verhindert, dass es sich wiederholt.

## Blatt
```markdown
# Vorfall <n> · eröffnet <Datum Uhrzeit> · Status: offen | eingedämmt | geschlossen
Was: <was offengelegt wurde, mit internem Namen und Hash; nie der Wert>
Wo und seit wann: <Kanal, Datei oder Dienst · frühestmögliches Datum>
Wer es sehen konnte: <öffentlich | Kunden | Personal | niemand außerhalb des Teams> — Nachweis: <Protokoll oder Befehl>
Eindämmung: <was deaktiviert oder gekappt wurde, wann> — Nachweis: <…>
Was nicht mehr funktioniert und für wen: <…>
Betroffene personenbezogene Daten: ja | nein | nicht auszuschließen — warum
Verantwortlicher für die Daten: <Kunde | wir> · Benachrichtigung gesendet?: <Datum, von wem> | Entwurf in <Pfad>
Meldung an die Behörde (entscheidet der Verantwortliche): ja | nein — Grund
Maßnahmen: <…>
Lehre: <neue Regel oder Verbesserung>
```

## Beispiel
Ein API-Token taucht in einer Konfigurationsdatei auf, die in einem Repository veröffentlicht wurde. Eindämmen: Es wird ein
neues Token erzeugt, an allen Stellen eingesetzt, die es nutzen, und das alte widerrufen. Diagnostizieren: Das Protokoll des
Anbieters sagt, ob jemand das Token genutzt hat und seit wann. Dokumentieren: Blatt ausgefüllt, auch wenn keine personenbezogenen Daten vorliegen.
Lehre: Die Konfigurationsdatei gehört in `.gitignore`, und das Repository wird vor der Veröffentlichung geprüft.
