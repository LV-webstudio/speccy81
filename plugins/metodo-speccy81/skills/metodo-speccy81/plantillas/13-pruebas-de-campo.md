# Pruebas de campo · <proyecto> · <fecha>

## 1. Montaje (comprobar ANTES de empezar)
| Qué | Valor | ¿Comprobado? |
|---|---|---|
| Equipos y dispositivos (modelo, SO, versión de la app) | | |
| Cómo se arranca cada pieza (**desde un terminal limpio**, no desde otra sesión o proceso que herede variables) | | |
| Modo de permisos / configuración de cada sesión (p. ej. sin modo automático si se prueban aprobaciones) | | |
| Ajustes que la prueba necesita activos (p. ej. avisos push, Remote Control, depuración USB) | | |
| Datos de prueba (reales o de semilla; nunca datos personales en capturas que se guarden) | | |
| Quién ejecuta y quién observa (usuario / sesión / otro equipo) | | |
| Cómo se observa (capturas, ADB, registros, `dumpsys`, consola) | | |
| **Puerta «compila»:** comprobación de tipos y build de producción en verde sobre el commit que se prueba (el servidor de desarrollo no lo garantiza) | | |

## 2. Pruebas
| # | Prueba | Qué confirma | Pasos | Resultado esperado | Prioridad |
|---|---|---|---|---|---|
| P1 | | | | | Alta |

## 3. Resultados
| # | Resultado (✅ / ❌ / ⚠ no válida) | Hora | Evidencia (captura, salida) | Detalle |
|---|---|---|---|---|
| P1 | | | | |

«⚠ no válida» = el montaje no cumplía la tabla 1; se repite, no cuenta como fallo del producto.

**Una prueba que falla no se salta:** se repite (p. ej. 3 veces) para saber si es inestable o real, se mira la captura y se averigua si falla la prueba o la app. Si al final se salta, consta como «saltada» y con el motivo.

## 4. Hallazgos y cambios
| Hallazgo | Afecta a (regla / documento / código) | Cambio hecho a la vez |
|---|---|---|
| | | |

## 5. Pendiente de repetir
-
