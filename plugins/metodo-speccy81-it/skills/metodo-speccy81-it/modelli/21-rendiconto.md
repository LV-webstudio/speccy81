# Rendiconto (regola 2)

Chiude **ogni** incarico, anche se breve. Va all'utente o alla coordinatrice (e, con Wassup, al diretto e alla
casella di posta). Se manca qualche sezione, l'incarico resta «non rendicontato».

## Formato
```markdown
## Rendiconto · <incarico> · <data e ora>
Ordine (alla lettera): «<testo esatto dell'ordine, con chi lo ha dato e in quale finestra>»
Fatto:
- <cosa è stato fatto, una riga per cosa>
Prova: <commit, impronta SHA-256, percorso, riga di registro o output di un comando>
Prova: <una per ogni cosa fatta; vale anche con il punto elenco: «- Prova: …»>
Non fatto: <cosa non è stato fatto> — <perché (blocco dei permessi, manca un dato, fuori perimetro)>
Non verificato: <ciò che si afferma senza averlo verificato> | niente
```

## Regole
- La riga inizia con `Prova:` (o `- Prova:`). Etichetta per lingua: es Prueba · en Proof · ca, pt e it Prova ·
  fr Preuve (con spazio prima di «:») · de Nachweis · nl Bewijs · pl Dowód.
- Le parole **fatto, verificato, caricato, distribuito, cancellato, installato, pubblicato e applicato** senza una
  `Prova:` nella stessa sezione sono un avviso.
- Una prova è qualcosa che un altro può tornare a guardare: «l'ho visto» non è una prova; «l'ha salvato l'app» nemmeno, se
  non è stato riletto nella destinazione.
- Ciò che non si è potuto provare si dice in «Non verificato», con chi deve farlo (p. es. «iPhone reale: in attesa del
  dispositivo»).
- Se poi compare un errore in qualcosa di già rendicontato, **errata corrige** con la stessa intestazione e «Corregge: <data>».

## Esempio
```markdown
## Rendiconto · indice della guida · 01-03-2026 10:40
Ordine (alla lettera): «Correggi i link rotti dell'indice» (utente, nella finestra di costruzione)
Fatto:
- 3 link corretti in GUIDA.md
Prova: commit 4f2a9c1
Prova: `valida-conoscenza.sh` → «0 link rotti»
Non fatto: l'indice del README inglese — non è di questa sessione (proprietario: revisione)
Non verificato: niente
```
