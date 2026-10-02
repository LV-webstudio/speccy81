# Mémoire idempotente (règle 11)

## Principes
- **Un sujet par fichier** et un **index court** (`MEMORY.md` : une ligne par fichier).
- **Fichiers d'état** (ce qui change) : **réécrits intégralement** avec « État au <date et heure> », jamais avec du texte
  ajouté à la fin. **Fichiers de décision** (ce qui est stable) : on n'y touche pas, sauf si la décision change.
- **Un `reprendre.md`** comme point d'entrée. Il est réécrit à la clôture de chaque phase ou bloc, et toujours avant de
  redémarrer une longue session (au lieu de compacter).
- Liens entre fichiers avec `[[nom]]`. Rien de ce que le dépôt conserve déjà (code, historique git).
- **Pas de secrets ni de données de tiers.** Les données de l'utilisateur lui-même, uniquement dans la mémoire locale.
- **Compacter seulement à la clôture d'un bloc**, avec la mémoire déjà enregistrée ; si cela arrive tout seul, on reprend depuis `reprendre.md`.

## Modèle de `reprendre.md`
```markdown
---
name: reprendre
description: COMMENCER ICI à l'ouverture d'une nouvelle session sur <projet> : où en était le travail, fils ouverts et quoi vérifier en premier
metadata:
  type: project
---

**État au <date heure>.** Fichier idempotent : réécrit intégralement à la clôture de chaque bloc.

## Quoi vérifier en premier (5 minutes)
1. <dernier commit / arbre propre>
2. <boîte aux lettres ou état des autres machines>
3. <sessions actives et leurs noms>

## Fils ouverts (dans l'ordre)
| # | Fil | Étape suivante | Où |
|---|---|---|---|

## Règles de travail qui ne changent pas
- <les règles inviolables du projet>
```

## Modèle de fichier d'état
```markdown
---
name: <sujet>
description: <une ligne pour décider s'il est pertinent>
metadata:
  type: project
---

**État au <date heure>.** Réécrit intégralement.

- <fait> · <où> · <en attente> · <décision attendue de l'utilisateur>

Voir [[reprendre]].
```

## Index (`MEMORY.md`)
```markdown
- [REPRENDRE · commencer ici](reprendre.md) — où en était le travail et quoi vérifier
- [<Sujet>](<sujet>.md) — <accroche d'une ligne>

Fichiers d'état (…) : ils sont RÉÉCRITS intégralement à la clôture de chaque bloc. Les autres sont des décisions stables.
```
