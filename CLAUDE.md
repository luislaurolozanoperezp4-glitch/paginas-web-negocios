# Reglas de guardado

- Todo archivo que Claude cree o modifique en una sesión se guarda en este repositorio: hacer commit y push al terminar cada tarea, sin esperar a que el usuario lo pida.
- Excepción: los archivos que el usuario diga expresamente que NO se guarden. Esos se quedan fuera (no se agregan al commit).
- Antes de cerrar o dar por terminada una sesión, confirmar con `git status` que no quedó nada sin subir, y decirle al usuario qué se guardó y qué no.
- Si el push falla (permisos, red), avisar de inmediato y mandar los archivos al usuario como descarga para que no se pierdan.
- Los archivos del entorno son temporales: nunca decir que algo "está guardado" hasta verificar que está en GitHub.

# Guardar todo, no solo archivos

- Al terminar cada sesión, crear `sesiones/AAAA-MM-DD-tema.md` con: qué se pidió, qué se hizo, decisiones, datos importantes que Claude dio como respuesta (listas, explicaciones, pendientes) y los enlaces usados. Así el texto de la conversación también queda guardado.
- Guardar también los archivos auxiliares (scripts generadores, fotos originales, borradores), no solo el resultado final.
- Subir todo con commit y push, salvo lo que el usuario excluya expresamente.
