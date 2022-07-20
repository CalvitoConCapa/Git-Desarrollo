# CLASE - 03

## GIT BRANCH

> para ver las ramas

*   git branch


> Para crear una rama

*   git branch <nombre-rama>
*   EJ: git branch dev


> Para cambiar de rama

*   git switch <nombre-de-la-rama>
*   EJ: git switch dev

> Borrar rama

*   git branch -d <nombre-de-la-rama>
*   EJ: git branch -d dev


## GIT MERGE (FUNCIONES DE RAMA)
**IMPORTANTE**
> Siempre tengo que estar en la rama en la que quiero recibir los cambios. EJ: si, en master, quiero recibir los cambios que hice en dev, tengo que estar en master.


### TIPOS DE MARGE

* Fast-Foodward - (No hay nungun conflicto, se hace de forma automatica)
* Recursivo - Uniones automaticas - (Tampoco hay conflictos) - Trabaja con el algoritmo
* Manual - (Donde hay conflictos - Y aca es donn hay que juntarse para resolver el conflicto)