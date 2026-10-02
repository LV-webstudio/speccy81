# Análisis de huecos · «¿qué falta para hacerlo con calidad?»

Pregunta guía: *¿qué determina la calidad del resultado final que ve el cliente, y está cubierto con
datos concretos que un motor pueda aplicar?*

Para cada tema: buscar en `conocimiento/` (grep de términos clave) y marcar.

| Tema | Términos para buscar | Docs que lo cubren | ¿Suficiente para calcular? | Acción |
|---|---|---|---|---|
| Cómo se ejecuta el trabajo paso a paso (técnica) | | | | |
| Parámetros numéricos (velocidades, tiempos, tamaños, márgenes) | | | | |
| Qué se puede y no se puede controlar de las herramientas/equipos | | | | |
| Simulación o validación antes de hacerlo en real | | | | |
| Condiciones externas (tiempo, luz, horario, temporada) | | | | |
| Seguridad, emergencias e incidentes | | | | |
| Casos límite (entornos difíciles, fallos) | | | | |
| Post-proceso y entrega (formatos, control de calidad) | | | | |
| Automatización del post-proceso | | | | |
| Ejemplos reales (ficheros, muestras) | | | | |
| Formación del equipo | | | | |
| Riesgos laborales y legales específicos | | | | |
| **Pruebas con datos o uso reales** (¿existe un banco mínimo? ¿se ha probado ya?) | | | | |
| **Privacidad y datos mínimos** (qué se lee, guarda y envía; RGPD) | | | | |
| **Despliegue y sistemas existentes** (dónde vive, con qué se conecta, qué pasa si se muda) | | | | |

Solo los huecos reales generan un bloque de investigación nuevo. Repetir hasta que no queden
huecos importantes. Todo lo que dependa de las condiciones (clima, luz, datos del cliente) debe
acabar en un **selector** con reglas, no en texto suelto.
