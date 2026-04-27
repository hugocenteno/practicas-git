# Limpieza de commits con rebase interactivo

En esta tarea he utilizado `git rebase -i` para limpiar el historial de commits del repositorio.

Primero creé varios commits con mensajes poco descriptivos, como “Cambios”, “Arreglos” y “Actualización de cosas”. Estos mensajes no explicaban claramente qué se había modificado, por lo que el historial no era fácil de entender.

Después ejecuté el comando `git rebase -i HEAD~3` para abrir el rebase interactivo sobre los tres últimos commits. En el editor mantuve el primer commit con `pick` y fusioné los otros dos con `squash`.

Finalmente cambié el mensaje resultante por uno más claro y descriptivo: “Mejora del archivo.txt con varios cambios organizados”. Después actualicé el repositorio remoto usando `git push origin main --force`, ya que el historial había sido reescrito.

Este proceso permite mantener un historial más limpio y profesional, con commits que explican mejor los cambios realizados.
