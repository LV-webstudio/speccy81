# Método Speccy81

![Speccy81 Method](assets/banner.jpg)

**De la idea al lanzamiento.** Un método de LV-Webstudio (Speccy81) para plantear cualquier proyecto (producto, servicio, módulo o app) con el mismo rigor: investigar primero, decidir con datos, convertir lo aprendido en conocimiento verificado, auditarlo, diseñar antes de programar, probar en el campo y publicar sin sorpresas. Tiene dos ediciones construidas desde el mismo método, cada una como marketplace de plugins de Claude Code.

Esta es la **edición básica**: libre y pública, con una skill, una guía corta y 8 plantillas en cada idioma.

**Languages · Idiomas:** [English](README.md) · [Español](README.es.md) · [Català](README.ca.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Português](README.pt.md) · [Français](README.fr.md) · [Italiano](README.it.md) · [Deutsch](README.de.md)

## Ediciones

| | Básica | Completa |
|---|---|---|
| Licencia | Pública: CC BY 4.0 (guía, SKILL y plantillas) + MIT (scripts); ver `NOTICE` | Propietaria, de LV-Webstudio |
| Recorrido | Un recorrido ligero de cinco pasos para ampliaciones y proyectos pequeños | Fases 0–9 más la 8 bis |
| Plantillas | 8 (01, 06, 09, 10, 13, 15, 20 y 21) | 21 |
| Reglas de oro | Las 13, en corto | Las 13 enteras, más las mejoras de eficiencia E1–E15 |
| Investigación y auditoría | — | Oleadas de investigación en paralelo y una auditoría única |
| Validador de conocimiento | — | Sí |
| Despliegue y lanzamiento | — | Despliegue y QA en otro dispositivo, y publicación |
| Gobierno y seguridad | Regla 13 en corto, «Prueba:» en todo resultado, incidentes (20) y rendición de cuentas (21) | Además: gobierno de varios equipos (19), trasladar un secreto y rotar una clave expuesta |
| Varios equipos | Una sola sesión o equipo; para varias sesiones con reglas mínimas, Wassup Básica | Gobierno completo y coordinación opcional con Wassup |

## Los cinco pasos

| Paso | Qué se hace | Plantilla |
|---|---|---|
| 1 · Fase 0 | Ficha de contexto; si el proyecto ya está empezado, se recoge lo que existe (código, documentos, decisiones) | 01 |
| 2 | Checklist de huecos y hechos canónicos, antes de investigar o diseñar | 06, 10 |
| 3 · Fase 7 | Diseño corto, aprobado por el usuario antes de programar | 09 |
| 4 · Fase 8 | Construcción con pruebas reales y de campo | 13 |
| 5 | Memoria idempotente al cerrar cada paso | 15 |
| Siempre | Rendición de cuentas con «Prueba:» al cerrar cada encargo; incidente si se expone una clave o un dato | 21, 20 |

La numeración de las fases (0, 7 y 8) es la del método completo, para que el proyecto pueda crecer sin renumerar nada. La edición completa añade el resto: las fases 1 a 6, la 8 bis y la 9.

## Qué contiene

Un plugin por idioma, cada uno con la skill, la guía y las 8 plantillas: `speccy81-method` (English), `metodo-speccy81` (Español), `metode-speccy81-ca` (Català), `metodo-speccy81-pt` (Português), `methode-speccy81-fr` (Français), `metodo-speccy81-it` (Italiano), `speccy81-methode-de` (Deutsch), `speccy81-methode-nl` (Nederlands) y `metoda-speccy81-pl` (Polski).

Todos los plugins llevan el mismo método; instala el del idioma que prefieras.

## Instalación

```
claude plugin marketplace add LV-webstudio/speccy81
claude plugin install speccy81-method@speccy81      # English
claude plugin install metodo-speccy81@speccy81      # Español
claude plugin install metode-speccy81-ca@speccy81   # Català
claude plugin install metodo-speccy81-pt@speccy81   # Português
claude plugin install methode-speccy81-fr@speccy81  # Français
claude plugin install metodo-speccy81-it@speccy81   # Italiano
claude plugin install speccy81-methode-de@speccy81  # Deutsch
claude plugin install speccy81-methode-nl@speccy81  # Nederlands
claude plugin install metoda-speccy81-pl@speccy81   # Polski
```

Después pídele a Claude Code «aplica el método Speccy81», también para un proyecto ya empezado. La skill carga la guía y las plantillas cuando hacen falta.

[Wassup](https://github.com/LV-webstudio/wassup) es un complemento opcional cuando varios equipos o sesiones trabajan en el mismo proyecto.

## Cómo conseguir la edición completa

La edición completa tiene licencia de LV-Webstudio. Pide acceso a través de [lv-webstudio.com](https://lv-webstudio.com/).

## Licencia

La edición básica se ofrece con dos licencias: **CC BY 4.0** para la guía, SKILL.md y las plantillas (uso libre, también comercial, citando la autoría) y **MIT** para los scripts y el código. Atribución sugerida: «Método Speccy81 · LV-Webstudio · lv-webstudio.com». La edición completa no está cubierta por estas licencias. Consulta [LICENSE](LICENSE).
