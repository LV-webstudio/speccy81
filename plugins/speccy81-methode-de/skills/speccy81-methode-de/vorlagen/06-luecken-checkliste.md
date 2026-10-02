# Lückenanalyse · «Was fehlt, um das in Qualität zu machen?»

Leitfrage: *Was bestimmt die Qualität des Endergebnisses, das der Kunde sieht, und ist es
mit konkreten Daten abgedeckt, die eine Engine anwenden kann?*

Für jedes Thema: `wissen/` durchsuchen (grep nach Schlüsselbegriffen) und abhaken.

| Thema | Suchbegriffe | Dokumente, die es abdecken | Genug zum Rechnen? | Maßnahme |
|---|---|---|---|---|
| Wie die Arbeit Schritt für Schritt ausgeführt wird (Technik) | | | | |
| Numerische Parameter (Geschwindigkeiten, Zeiten, Größen, Toleranzen) | | | | |
| Was sich an Werkzeugen/Ausrüstung steuern lässt und was nicht | | | | |
| Simulation oder Validierung vor der echten Ausführung | | | | |
| Äußere Bedingungen (Wetter, Licht, Tageszeit, Jahreszeit) | | | | |
| Sicherheit, Notfälle und Zwischenfälle | | | | |
| Grenzfälle (schwierige Umgebungen, Ausfälle) | | | | |
| Nachbearbeitung und Auslieferung (Formate, Qualitätskontrolle) | | | | |
| Automatisierung der Nachbearbeitung | | | | |
| Echte Beispiele (Dateien, Muster) | | | | |
| Schulung des Teams | | | | |
| Spezifische arbeits- und rechtsbezogene Risiken | | | | |
| **Tests mit echten Daten oder im echten Einsatz** (gibt es eine minimale Testbank? wurde es schon ausprobiert?) | | | | |
| **Datenschutz und Datenminimierung** (was gelesen, gespeichert und gesendet wird; DSGVO) | | | | |
| **Deployment und bestehende Systeme** (wo es läuft, womit es verbunden ist, was passiert, wenn es umzieht) | | | | |

Nur echte Lücken erzeugen einen neuen Rechercheblock. Wiederholen, bis keine wichtigen Lücken
mehr bleiben. Alles, was von Bedingungen abhängt (Wetter, Licht, Kundendaten), muss
in einem **Selektor** mit Regeln landen, nicht in losem Text.
