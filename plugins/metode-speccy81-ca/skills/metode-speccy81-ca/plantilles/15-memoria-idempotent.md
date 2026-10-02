# Memòria idempotent (regla 11)

## Principis
- **Un tema per fitxer** i un **índex curt** (`MEMORY.md`: una línia per fitxer).
- **Fitxers d'estat** (el que canvia): **reescrits sencers** amb «Estat a data de <data i hora>», mai amb text
  afegit al final. **Fitxers de decisió** (el que és estable): no es toquen tret que la decisió canviï.
- **Un `reprendre.md`** com a punt d'entrada. Es reescriu en tancar cada fase o bloc, i sempre abans de
  reiniciar una sessió llarga (en lloc de compactar).
- Enllaços entre fitxers amb `[[nom]]`. Res del que ja guarda el repositori (codi, historial de git).
- **Sense secrets ni dades de tercers.** Les dades de l'usuari mateix, només a la memòria local.
- **Compactar només en tancar un bloc**, amb la memòria ja desada; si arriba sola, es reprèn des de `reprendre.md`.

## Plantilla de `reprendre.md`
```markdown
---
name: resum
description: COMENÇA AQUÍ en obrir una sessió nova a <projecte>: on es va deixar, fils oberts i què comprovar primer
metadata:
  type: project
---

**Estat a data de <data hora>.** Fitxer idempotent: es reescriu sencer en tancar cada bloc.

## Què comprovar primer (5 minuts)
1. <últim commit / arbre net>
2. <bústia o estat de les altres màquines>
3. <sessions actives i els seus noms>

## Fils oberts (per ordre)
| # | Fil | Pas següent | On |
|---|---|---|---|

## Regles de treball que no canvien
- <les regles inviolables del projecte>
```

## Plantilla de fitxer d'estat
```markdown
---
name: <tema>
description: <una línia per decidir si és rellevant>
metadata:
  type: project
---

**Estat a data de <data hora>.** Reescrit sencer.

- <fet> · <on> · <pendent> · <decisió que espera l'usuari>

Vegeu [[resum]].
```

## Índex (`MEMORY.md`)
```markdown
- [REPRENDRE · comença aquí](reprendre.md) — on es va deixar la feina i què comprovar
- [<Tema>](<tema>.md) — <ganxo d'una línia>

Fitxers d'estat (…): es REESCRIUEN sencers en tancar cada bloc. La resta són decisions estables.
```
