# Flujo de trabajo — Learn Git Branching

> Cada integrante completa su propia fila con lo observado durante la práctica individual, después de resolver los niveles obligatorios.

## Registro de comandos

| Comando | Pregunta de observación | Observación (ejemplo a completar por cada integrante) |
|---|---|---|
| `git commit` | ¿Qué nodo nuevo apareció y dónde quedó apuntando la rama? | Apareció un nuevo nodo (círculo) conectado al commit anterior, y la rama activa se movió automáticamente para apuntar a ese nuevo nodo. |
| `git branch` | ¿Qué se creó y sobre qué commit quedó ubicado? | Se creó una nueva etiqueta de rama sobre el commit en el que se estaba parado en ese momento; no se movió ningún nodo, solo se agregó la referencia. |
| `git checkout` | ¿Qué cambió al moverse a otra rama? | El puntero especial `HEAD` se movió a la rama indicada, por lo que los commits siguientes ya no afectarán a la rama anterior sino a la nueva rama activa. |
| `git merge` | ¿Qué historias de trabajo quedaron integradas? | Los commits exclusivos de la rama fusionada quedaron combinados en la rama destino, creando un nuevo commit de fusión que tiene dos padres cuando las historias habían divergido. |

## Explicación de una línea por comando (para cada integrante)

- `git commit`: guarda una nueva fotografía del proyecto con un mensaje explicativo.
- `git branch`: crea una línea de trabajo independiente sin cambiar de posición actual.
- `git checkout`: cambia el punto de trabajo activo hacia otra rama o commit.
- `git merge`: une el historial de dos ramas en una sola.

*(Espacio para que cada integrante agregue su propia línea si usó comandos adicionales durante los niveles: por ejemplo `git checkout -b`, `git log`, etc.)*

## Evidencia
Adjuntar en `evidencias/` una captura por integrante que muestre los niveles obligatorios completados:
- `evidencias/learn-git-usuario1.png`
- `evidencias/learn-git-usuario2.png`
- `evidencias/learn-git-usuario3.png`
