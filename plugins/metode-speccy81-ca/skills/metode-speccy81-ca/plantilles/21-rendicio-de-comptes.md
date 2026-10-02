# Rendició de comptes (regla 2)

Tanca **cada** encàrrec, encara que sigui curt. Va a l'usuari o a la coordinadora (i, amb Wassup, al directe i a la
bústia). Si falta algun apartat, l'encàrrec queda «sense rendir».

## Format
```markdown
## Rendició de comptes · <encàrrec> · <data i hora>
Ordre (literal): «<text exacte de l'ordre, amb qui la va donar i a quina finestra>»
Fet:
- <què s'ha fet, una línia per cosa>
Prova: <commit, empremta SHA-256, ruta, línia de registre o sortida d'una ordre>
Prova: <una per cada cosa feta; val amb vinyeta: «- Prova: …»>
No fet: <què no s'ha fet> — <per què (bloqueig de permisos, falta una dada, fora d'abast)>
Sense comprovar: <el que s'afirma sense haver-ho comprovat> | res
```

## Regles
- La línia comença per `Prova:` (o `- Prova:`). Etiqueta per idioma: es Prueba · en Proof · ca, pt i it Prova ·
  fr Preuve (amb espai abans de «:») · de Nachweis · nl Bewijs · pl Dowód.
- Les paraules **fet, comprovat, pujat, desplegat, esborrat, instal·lat, publicat i aplicat** sense una
  `Prova:` al mateix apartat són un avís.
- Una prova és una cosa que un altre pot tornar a mirar: «ho he vist» no és prova; «ho va desar l'app» tampoc, si no
  s'ha rellegit al destí.
- El que no es va poder provar es diu a «Sense comprovar», amb qui ho ha de fer (p. ex. «iPhone real: pendent de
  dispositiu»).
- Si després apareix un error en alguna cosa rendida, **fe d'errates** amb la mateixa capçalera i «Corregeix a: <data>».

## Exemple
```markdown
## Rendició de comptes · índex de la guia · 01-03-2026 10:40
Ordre (literal): «Corregeix els enllaços trencats de l'índex» (usuari, a la finestra de construcció)
Fet:
- 3 enllaços corregits a GUIA.md
Prova: commit 4f2a9c1
Prova: `validar-coneixement.sh` → «0 enllaços trencats»
No fet: l'índex del README anglès — no és d'aquesta sessió (propietari: revisió)
Sense comprovar: res
```
