# Incidente de seguridad (clave, dato o canal expuestos)

Se abre en cuanto se sospecha, sin esperar a estar seguro. Sin secretos ni datos personales en este documento:
de las claves, solo su nombre interno y su huella; de las personas, solo su papel.

## Pasos
1. **Contener** lo urgente: desactivar la clave, cortar el acceso o el canal. Si es una clave, con la regla de la
   clave expuesta: la sustituta primero; si es pública y urgente, se desactiva ya diciendo antes qué deja de
   funcionar y para quién. Nunca se reactiva.
2. **Diagnosticar solo leyendo:** qué quedó expuesto, desde cuándo, dónde y quién pudo verlo. Se mide (regla 2):
   cifra, consulta o comando, fecha.
3. **Decidir y avisar:** decide el usuario. Si hay datos personales de un cliente, el cliente es el **responsable**
   y tú el **encargado**: le avisas por escrito **sin dilación indebida** (art. 33.2 RGPD) con qué pasó, desde
   cuándo, qué se ha hecho y qué no se puede descartar. El responsable valora si notifica a la autoridad de
   protección de datos en **72 horas** (art. 33). Si los datos son tuyos, el responsable eres tú.
4. **Registrar** todo incidente, aunque no se notifique (art. 33.5): hechos, efectos y medidas.
5. **Lección:** la regla nueva o la mejora del método que evita que se repita.

## Ficha
```markdown
# Incidente <n> · abierto <fecha hora> · estado: abierto | contenido | cerrado
Qué: <qué quedó expuesto, por nombre interno y huella; nunca el valor>
Dónde y desde cuándo: <canal, fichero o servicio · primera fecha posible>
Quién pudo verlo: <público | clientes | personal | nadie fuera del equipo> — Prueba: <registro o comando>
Contención: <qué se desactivó o cortó, cuándo> — Prueba: <…>
Qué deja de funcionar y para quién: <…>
Datos personales afectados: sí | no | no se puede descartar — por qué
Responsable de los datos: <cliente | nosotros> · ¿aviso enviado?: <fecha, por quién> | borrador en <ruta>
Notificación a la autoridad (la decide el responsable): sí | no — motivo
Medidas: <…>
Lección: <regla nueva o mejora>
```

## Ejemplo
Un token de una API aparece en un fichero de configuración que se publicó en un repositorio. Contener: se genera
un token nuevo, se pone en todos los sitios que lo usan y se revoca el viejo. Diagnosticar: el registro del
proveedor dice si alguien usó el token y desde cuándo. Registrar: ficha rellena aunque no haya datos personales.
Lección: el fichero de configuración va en `.gitignore` y el repositorio se revisa antes de publicar.
