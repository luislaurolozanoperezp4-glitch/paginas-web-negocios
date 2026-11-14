# Reglas de guardado

## Por defecto
- Los archivos que Claude cree o modifique en una sesión se guardan en este repositorio: commit y push al terminar cada tarea, sin esperar a que el usuario lo pida.
- Excepción: lo que el usuario diga expresamente que NO se guarde se queda fuera del commit.
- Al terminar una sesión, guardar un resumen corto en `sesiones/AAAA-MM-DD-tema.md` (qué se pidió, qué se hizo, pendientes).

## Verificación
- Nunca decir que algo "está guardado" hasta comprobar con `git status` y `git log` que está subido.
- Al cerrar, decirle al usuario qué se guardó y qué no.
- Si el push falla (permisos, red), avisar de inmediato y mandar los archivos como descarga.

## Cuidado
- No subir contraseñas, tokens, claves ni datos privados de personas que no sean necesarios para el trabajo.
- Si el repositorio es público, avisar antes de subir datos personales (teléfonos, cédulas, fotos de personas) y recomendar pasarlo a privado.
- Los archivos del entorno de Claude son temporales: lo que no esté en GitHub o descargado se pierde.
