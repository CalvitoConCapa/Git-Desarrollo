# CLASE - 04
ONEPIECE276
# .gitkeep: Versionar carpetas
Creo un archivo vacío llamado ".gitkeep" dentro de la carpeta que quiero versionar

## Alias
Forma resumida para llamar a un comando

git config --global alias.l "log --online"
git config --global alias.s "status --short"
git config --global alias.ll "log --onegline --decorate --all --graph"

## Ver alias disponibles

git config --get-regexp alias

## Para borrar un alias

git config --global --unset alias.
EJ: git config --global --unset alias.s

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

# GIT STASH
**NOTA**: Los stash no estan disponibles en el remoto. SOLO en el LOCAL. No se sube al remoto.


### Crear un stash

    git stash

### Veo los stash

    git stash list

### Para borrar un stash

> borrar el ultimo stash

    git stash drop

> Borrar un stash particular

    git stash drop <stash>

> Aplicar un stash, el ultimo

    git stash pop

> Aplicar cualquier stash de los que tengo

    git stash apply
    git stash apply stash@{1}

## GIT RESET

> SOFT: me saca los commit y me deja todo en el Staging AREA

    git reset --soft (lo deja es el stegin area [add .])

> MIXED: Me saca los commits y me los deja en el Working DIRECTORY

    git reset <número-hash>
    git resen --mixed (lo lleva al working directori)

> HARD(Peligroso, muito cudado): Borra los commits difinitivamente y los cambios

    git reset hard
