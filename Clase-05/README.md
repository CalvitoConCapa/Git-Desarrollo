# Clase - 05

## Trabajar em proyectos Open Source (Pull Request)

1. Hacer un fork del proyecto. (Me copia el repo a mi cuenta de github).
2. Me clono el fork desde mi cuenta de githun.
3. Trabajo normalmente. Subo los cambios.
4. Me voy al proyecto original en el apartado Pull Request. Creo uno nuevo.
5. Una vez aceptado, tengo que actualizar mi fork.
6. Voy a la cuenta del proyecto original y me copio la url del repositorio.
7. Agrego la url del repositorio original a mi repo local

    git remote upstream <URL-repositorio-original>

8. Me traigo los cambios

    git pull upstream <rama-que-quiero-actualizar>

9. Subir esas actualizaciones del repositorio local a mi remoto.