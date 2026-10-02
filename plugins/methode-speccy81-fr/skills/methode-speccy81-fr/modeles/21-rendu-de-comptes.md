# Rendu de comptes (règle 2)

Clôt **chaque** mandat, même court. Il va à l'utilisateur ou au coordinateur (et, avec Wassup, au direct et à la boîte
aux lettres). S'il manque une rubrique, le mandat reste « sans rendu ».

## Format
```markdown
## Rendu de comptes · <mandat> · <date et heure>
Ordre (littéral) : « <texte exact de l'ordre, avec qui l'a donné et dans quelle fenêtre> »
Fait :
- <ce qui a été fait, une ligne par chose>
Preuve : <commit, empreinte SHA-256, chemin, ligne de journal ou sortie d'une commande>
Preuve : <une pour chaque chose faite ; vaut aussi avec une puce : « - Preuve : … »>
Non fait : <ce qui n'a pas été fait> — <pourquoi (blocage d'autorisations, donnée manquante, hors périmètre)>
Non vérifié : <ce qui est affirmé sans l'avoir vérifié> | rien
```

## Règles
- La ligne commence par `Preuve :` (ou `- Preuve :`). Étiquette par langue : es Prueba · en Proof · ca, pt et it Prova ·
  fr Preuve (avec une espace avant « : ») · de Nachweis · nl Bewijs · pl Dowód.
- Les mots **fait, vérifié, téléversé, déployé, supprimé, installé, publié et appliqué** sans une
  `Preuve :` dans la même rubrique sont un avertissement.
- Une preuve est quelque chose qu'un autre peut regarder à nouveau : « je l'ai vu » n'est pas une preuve ; « l'app l'a enregistré » non plus, si
  on ne l'a pas relu à la destination.
- Ce qui n'a pas pu être prouvé se dit dans « Non vérifié », avec qui doit le faire (p. ex. « iPhone réel : en attente
  d'appareil »).
- Si une erreur apparaît ensuite dans quelque chose de rendu, **erratum** avec le même en-tête et « Corrige : <date> ».

## Exemple
```markdown
## Rendu de comptes · index du guide · 01-03-2026 10:40
Ordre (littéral) : « Corrige les liens cassés de l'index » (utilisateur, dans la fenêtre de construction)
Fait :
- 3 liens corrigés dans GUIDE.md
Preuve : commit 4f2a9c1
Preuve : `valider-connaissances.sh` → « 0 lien cassé »
Non fait : l'index du README anglais — il n'est pas de cette session (propriétaire : revue)
Non vérifié : rien
```
