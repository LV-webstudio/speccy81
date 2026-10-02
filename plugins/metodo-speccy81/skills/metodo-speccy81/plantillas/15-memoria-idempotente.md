# Memoria idempotente (regla 11)

## Principios
- **Un tema por fichero** y un **índice corto** (`MEMORY.md`: una línea por fichero).
- **Ficheros de estado** (lo que cambia): se **reescriben enteros** con «Estado a <fecha y hora>», nunca se les
  añade texto al final. **Ficheros de decisión** (lo estable): no se tocan salvo que la decisión cambie.
- **Un `retomar.md`** como puerta de entrada. Se reescribe al cerrar cada fase o bloque, y siempre antes de
  reiniciar una sesión larga (en lugar de compactar).
- Enlaces entre ficheros con `[[nombre]]`. Nada que ya guarde el repositorio (código, historial de git).
- **Sin secretos ni datos de terceros.** Los datos del propio usuario, solo en la memoria local.
- **Compactar solo al cerrar un bloque**, con la memoria ya guardada; si llega sola, se retoma desde `retomar.md`.

## Plantilla de `retomar.md`
```markdown
---
name: retomar
description: EMPIEZA AQUÍ al abrir una sesión nueva en <proyecto>: dónde se quedó, hilos abiertos y qué comprobar primero
metadata:
  type: project
---

**Estado a <fecha hora>.** Fichero idempotente: se reescribe entero al cerrar cada bloque.

## Qué comprobar primero (5 minutos)
1. <último commit / árbol limpio>
2. <buzón o estado de otros equipos>
3. <sesiones activas y sus nombres>

## Hilos abiertos (por orden)
| # | Hilo | Siguiente paso | Dónde |
|---|---|---|---|

## Reglas de trabajo que no cambian
- <reglas inviolables del proyecto>
```

## Plantilla de fichero de estado
```markdown
---
name: <tema>
description: <una línea para decidir si es relevante>
metadata:
  type: project
---

**Estado a <fecha hora>.** Se reescribe entero.

- <hecho> · <dónde> · <pendiente> · <decisión que espera al usuario>

Ver [[retomar]].
```

## Índice (`MEMORY.md`)
```markdown
- [RETOMAR · empieza aquí](retomar.md) — dónde se quedó el trabajo y qué comprobar
- [<Tema>](<tema>.md) — <gancho de una línea>

Ficheros de estado (…): se REESCRIBEN enteros al cerrar cada bloque. Los demás son decisiones estables.
```
