# Veiligheidsincident (sleutel, gegeven of kanaal blootgesteld)

Wordt geopend zodra er een vermoeden is, zonder te wachten tot je zeker bent. Zonder geheimen of persoonsgegevens in dit document:
van de sleutels alleen hun interne naam en hun hash; van de personen alleen hun rol.

## Stappen
1. **Indammen** wat dringend is: de sleutel deactiveren, de toegang of het kanaal afsluiten. Als het een sleutel is, met de regel van de
   blootgestelde sleutel: de vervangende sleutel eerst; als hij openbaar en dringend is, wordt hij meteen gedeactiveerd nadat is
   gezegd wat ophoudt te werken en voor wie. Nooit weer activeren.
2. **Diagnosticeren alleen lezend:** wat is blootgesteld, sinds wanneer, waar en wie het kon zien. Er wordt gemeten (regel 2):
   getal, query of opdracht, datum.
3. **Beslissen en melden:** de gebruiker beslist. Als er persoonsgegevens van een klant zijn, is de klant de **verwerkingsverantwoordelijke**
   en ben jij de **verwerker**: je meldt dit de klant schriftelijk **zonder onredelijke vertraging** (art. 33 lid 2 AVG) met wat er is gebeurd, sinds
   wanneer, wat is gedaan en wat niet kan worden uitgesloten. De verwerkingsverantwoordelijke beoordeelt of hij het meldt aan de toezichthoudende
   autoriteit, binnen **72 uur** (art. 33 AVG). Als de gegevens van jou zijn, ben jij de verwerkingsverantwoordelijke.
4. **Registreren** van elk incident, ook als het niet wordt gemeld (art. 33 lid 5 AVG): feiten, gevolgen en maatregelen.
5. **Les:** de nieuwe regel of de verbetering van de methode die voorkomt dat het zich herhaalt.

## Formulier
```markdown
# Incident <n> · geopend <datum tijd> · status: open | ingedamd | gesloten
Wat: <wat is blootgesteld, met interne naam en hash; nooit de waarde>
Waar en sinds wanneer: <kanaal, bestand of dienst · eerst mogelijke datum>
Wie het kon zien: <openbaar | klanten | personeel | niemand buiten het team> — Bewijs: <log of opdracht>
Indamming: <wat is gedeactiveerd of afgesloten, wanneer> — Bewijs: <…>
Wat ophoudt te werken en voor wie: <…>
Getroffen persoonsgegevens: ja | nee | kan niet worden uitgesloten — waarom
Verantwoordelijke voor de gegevens: <klant | wij> · melding verzonden?: <datum, door wie> | concept in <pad>
Melding aan de autoriteit (beslist de verantwoordelijke): ja | nee — reden
Maatregelen: <…>
Les: <nieuwe regel of verbetering>
```

## Voorbeeld
Een API-token staat in een configuratiebestand dat in een repository is gepubliceerd. Indammen: er wordt een nieuw token gemaakt,
op alle plekken gezet die het gebruiken en het oude wordt ingetrokken. Diagnosticeren: het log van de aanbieder zegt of iemand het
token heeft gebruikt en sinds wanneer. Registreren: formulier ingevuld ook als er geen persoonsgegevens zijn.
Les: het configuratiebestand gaat in `.gitignore` en de repository wordt nagekeken vóór het publiceren.
