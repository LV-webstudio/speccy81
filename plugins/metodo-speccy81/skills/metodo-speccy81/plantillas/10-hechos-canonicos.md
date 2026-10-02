---
titulo: Hechos canónicos del dominio <dominio> · datos clave que todos los documentos deben usar igual
ambito: <dominio>
dominio: <dominio>
proyecto: comun
fuentes: <fuentes oficiales de cada dato>
fecha: AAAA-MM-DD
revisar: AAAA-MM-DD
estado: verificado
---

# Hechos canónicos · `00-HECHOS.md`

Se crea ANTES de lanzar la primera oleada de agentes. Todos lo leen al empezar.
Si un agente descubre un dato clave que afecta a otros bloques, lo añade aquí
(con fuente) y lo usa; si contradice uno existente, lo marca `⚠ en disputa` y
avisa en su informe. El coordinador resuelve las disputas.

## Premisas (con id)
Las suposiciones de las que dependen otros documentos llevan id (`P-…`). Los documentos y los encargos citan el id
entre corchetes (`[P-EQUIPO]`). Cuando una premisa cambia, se actualiza su fecha aquí y se revisan los documentos
que la citan con fecha anterior.
| Id | Premisa | Último cambio |
|---|---|---|
| P-EJEMPLO | <qué se da por supuesto> | AAAA-MM-DD |

## Decisiones tomadas
| Decisión | Valor | Fecha |
|---|---|---|

## Equipo y especificaciones clave
| Dato | Valor | Unidad | Fuente |
|---|---|---|---|

## Umbrales y reglas únicas (una sola cifra por dato)
| Regla | Valor | Documento canónico |
|---|---|---|

## Datos en disputa
| Dato | Valor A (fuente) | Valor B (fuente) | Quién lo resuelve |
|---|---|---|---|
