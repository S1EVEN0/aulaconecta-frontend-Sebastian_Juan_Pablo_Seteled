# Conceptos de Git y GitHub

## Comprobación conceptual

**1. ¿Qué puede hacer Git aunque GitHub no exista?**
Git puede funcionar completamente en un computador local, sin necesidad de internet ni de ninguna plataforma en línea. Permite guardar versiones de un proyecto, crear ramas, comparar cambios y volver a un estado anterior, todo dentro de la carpeta del proyecto. GitHub solo añade un lugar remoto donde alojar ese historial y facilita la colaboración entre varias personas.

**2. ¿Por qué una rama reduce el riesgo de dañar main?**
Porque los cambios se hacen en una copia paralela del proyecto que no afecta a `main` hasta que alguien decida integrarla. Si algo sale mal en la rama, se puede corregir, descartar o volver a intentar sin que la versión principal deje de funcionar en ningún momento.

**3. ¿Qué diferencia existe entre guardar un archivo y crear un commit?**
Guardar un archivo solo actualiza su contenido en el disco; esa versión anterior se pierde y no queda registro de qué cambió. Crear un commit, en cambio, congela una "foto" del proyecto en ese momento, con un mensaje que explica el propósito del cambio, y esa foto queda disponible para siempre en el historial, sin importar lo que se modifique después.

**4. ¿Por qué un pull request no es lo mismo que un merge?**
El pull request es la *solicitud* para que los cambios de una rama se integren a otra; es un espacio de conversación y revisión donde se puede comentar, pedir ajustes o aprobar. El merge es la *acción* de integrar realmente esos cambios. Puede existir un pull request abierto durante días sin que todavía se haya hecho merge.

**5. ¿Qué evidencia permite saber quién cambió algo y por qué?**
El historial de commits: cada commit queda asociado al usuario que lo hizo, a una fecha y a un mensaje que describe el cambio. Además, en un pull request queda registrada la conversación de revisión, lo que agrega el "por qué" detrás de cada corrección.

## Reto rápido de secuencia

Orden correcto de los pasos y riesgo que evita cada uno:

1. **Crear repositorio** — establece un único lugar central con historial, evitando copias sueltas del proyecto en distintos computadores.
2. **Crear rama** — separa el trabajo nuevo de la versión estable, evitando romper `main` mientras se experimenta.
3. **Hacer commits** — registra los cambios en pasos pequeños y explicados, evitando perder el rastro de qué se hizo y cuándo.
4. **Abrir pull request** — expone el cambio para que sea visible antes de integrarse, evitando que algo entre a `main` sin que nadie más lo sepa.
5. **Revisar** — permite que otra persona detecte errores, mejoras o riesgos que el autor no vio, evitando que un solo punto de vista decida la calidad del cambio.
6. **Corregir observaciones** — atiende lo señalado en la revisión, evitando fusionar un cambio incompleto o con errores conocidos.
7. **Fusionar (merge)** — integra el trabajo ya revisado y corregido en `main`, evitando que la rama de trabajo quede aislada del proyecto principal.
