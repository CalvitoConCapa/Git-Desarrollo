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

<------------------------------------------------------------------->

## TAG (Etiquetado)
Me permite etiquetar commits.

> Ver tags que tengo disponibles

    git tag

> Como creo un tag en el commit actual

    git tag v1.1

> Como creo un tag en un commit en especifico

    git tag v1.1 <hasg>
    
    git tag v1.1 <02fb9dd>

> Se usan los Tags: Con Versionado Semantico

    git tag -a v0.0.1 -m "Version 0.0.1"

    git tag -a v0.0.1 <hash> -m "Version 0.0.1"

    git tag -a v0.0.1 3eba1bc -m "Version 0.0.1"

*   a: Anotado
*   m: Mensaje

> Mostrar informacion detallada sobre los Tags

    git show v0.0.1


> Para borrar Tags

    git tag -d v0.0.1
    git tag -d <hash>

> Para subir todos los Tags (NO RECOMENDABLE)

    git push --tags

> Para suber un Tag en especifico

    git push origin <nombre-tag>

## GIT REBASE
Me reordena los commits y me los fusiona. Si me quiero traer los cambios de dev a master, tengoq ue estar sobre la rama master y hacer un:

    git rebase <rama-que-quiero-traer>
    git rebase <dev>

> Si tengo varios commits

    git rebase --continue