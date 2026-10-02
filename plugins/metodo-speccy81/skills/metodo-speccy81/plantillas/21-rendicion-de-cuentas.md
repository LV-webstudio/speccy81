# Rendición de cuentas (regla 2)

Cierra **cada** encargo, aunque sea corto. Va al usuario o a la coordinadora (y, con Wassup, al directo y al
buzón). Si falta algún apartado, el encargo queda «sin rendir».

## Formato
```markdown
## Rendición de cuentas · <encargo> · <fecha y hora>
Orden (literal): «<texto exacto de la orden, con quién la dio y en qué ventana>»
Hecho:
- <qué se hizo, una línea por cosa>
Prueba: <commit, huella SHA-256, ruta, línea de registro o salida de un comando>
Prueba: <una por cada cosa hecha; vale con viñeta: «- Prueba: …»>
No hecho: <qué no se hizo> — <por qué (bloqueo de permisos, falta un dato, fuera de alcance)>
Sin comprobar: <lo que se afirma sin haberlo comprobado> | nada
```

## Reglas
- La línea empieza por `Prueba:` (o `- Prueba:`). Etiqueta por idioma: es Prueba · en Proof · ca, pt e it Prova ·
  fr Preuve (con espacio antes de «:») · de Nachweis · nl Bewijs · pl Dowód.
- Las palabras **hecho, comprobado, subido, desplegado, borrado, instalado, publicado y aplicado** sin una
  `Prueba:` en el mismo apartado son un aviso.
- Una prueba es algo que otro puede volver a mirar: «lo he visto» no es prueba; «lo guardó la app» tampoco, si no
  se ha releído en el destino.
- Lo que no se pudo probar se dice en «Sin comprobar», con quién debe hacerlo (p. ej. «iPhone real: pendiente de
  dispositivo»).
- Si después aparece un error en algo rendido, **fe de erratas** con la misma cabecera y «Corrige a: <fecha>».

## Ejemplo
```markdown
## Rendición de cuentas · índice de la guía · 01-03-2026 10:40
Orden (literal): «Corrige los enlaces rotos del índice» (usuario, en la ventana de construcción)
Hecho:
- 3 enlaces corregidos en GUIA.md
Prueba: commit 4f2a9c1
Prueba: `validar-conocimiento.sh` → «0 enlaces rotos»
No hecho: el índice del README inglés — no es de esta sesión (dueño: revisión)
Sin comprobar: nada
```
