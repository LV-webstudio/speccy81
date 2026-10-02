# Incidente di sicurezza (chiave, dato o canale esposti)

Si apre appena lo si sospetta, senza aspettare di esserne certi. Senza segreti né dati personali in questo documento:
delle chiavi, solo il nome interno e l'impronta; delle persone, solo il ruolo.

## Passi
1. **Contenere** l'urgente: disattivare la chiave, interrompere l'accesso o il canale. Se è una chiave, con la regola della
   chiave esposta: prima la sostitutiva; se è pubblica e urgente, si disattiva subito dicendo prima cosa smette di
   funzionare e per chi. Non si riattiva mai.
2. **Diagnosticare solo leggendo:** cosa è rimasto esposto, da quando, dove e chi ha potuto vederlo. Si misura (regola 2):
   cifra, query o comando, data.
3. **Decidere e avvisare:** decide l'utente. Se ci sono dati personali di un cliente, il cliente è il **titolare**
   e tu il **responsabile**: lo avvisi per iscritto **senza ingiustificato ritardo** (art. 33.2 GDPR) con cosa è successo, da
   quando, cosa è stato fatto e cosa non si può escludere. Il titolare valuta se notificare all'autorità di
   protezione dei dati entro **72 ore** (art. 33). Se i dati sono tuoi, il titolare sei tu.
4. **Registrare** ogni incidente, anche se non si notifica (art. 33.5): fatti, effetti e misure.
5. **Lezione:** la regola nuova o il miglioramento del metodo che evita che si ripeta.

## Scheda
```markdown
# Incidente <n> · aperto <data ora> · stato: aperto | contenuto | chiuso
Cosa: <cosa è rimasto esposto, per nome interno e impronta; mai il valore>
Dove e da quando: <canale, file o servizio · prima data possibile>
Chi ha potuto vederlo: <pubblico | clienti | personale | nessuno fuori dal team> — Prova: <registro o comando>
Contenimento: <cosa è stato disattivato o interrotto, quando> — Prova: <…>
Cosa smette di funzionare e per chi: <…>
Dati personali coinvolti: sì | no | non si può escludere — perché
Titolare dei dati: <cliente | noi> · avviso inviato?: <data, da chi> | bozza in <percorso>
Notifica all'autorità (la decide il titolare): sì | no — motivo
Misure: <…>
Lezione: <regola nuova o miglioramento>
```

## Esempio
Un token di un'API compare in un file di configurazione che è stato pubblicato in un repository. Contenere: si genera
un token nuovo, lo si mette in tutti i luoghi che lo usano e si revoca il vecchio. Diagnosticare: il registro del
fornitore dice se qualcuno ha usato il token e da quando. Registrare: scheda compilata anche se non ci sono dati personali.
Lezione: il file di configurazione va in `.gitignore` e il repository si rivede prima di pubblicare.
