# Limpieza de commits con git rebase -i

## Objetivo

El objetivo de esta tarea fue limpiar el historial de commits utilizando `git rebase -i`, mejorando los mensajes y fusionando commits innecesarios.

## Commits iniciales

Se crearon commits con mensajes poco claros:

- Cambios
- Arreglos
- Actualización de cosas

Estos mensajes no describían correctamente los cambios realizados.

## Uso de rebase interactivo

Se ejecutó el siguiente comando:

git rebase -i HEAD~3

Este comando permitió modificar el historial de los últimos tres commits.

## Decisiones tomadas

Se utilizó la opción `reword` para cambiar el mensaje del primer commit y `squash` para fusionar los otros commits en uno solo.

El resultado fue un único commit con un mensaje más claro:

Mejorar y actualizar script de validación

## Push forzado

Después de reescribir el historial, se ejecutó:

git push --force

Esto fue necesario para actualizar el historial remoto en GitHub.
