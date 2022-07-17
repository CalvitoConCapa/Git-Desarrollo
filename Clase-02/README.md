# -----------------------
#  Clase-02 - 17/07/2022
# -----------------------

# EL <> SIGNIFICA QUE ES UNA VARIABLE (OSEA LO QUE CONTENGA PUEDE CAMBIAR DEPENDIENDO LA SITUACIÓN)

# Status de archivos

* UNTRACKED > Archivos que no se agregaron al index. O están en el Working Directory

* STAGED > Archivos que no fueron agregados al repositorio y cuyos cambios fueron validados.

* UNMODIFIED > Archivos que se encuentran en el repositorio y no fueron modificados.

* MODIFIEAD > Archivos que se encuentran en el repositorio pero difieren con lo que se encuentra en el Working Directory


## GIT LOG

Ayuda de git log

    git log --help

Muestra versión completa:
    
    git log

Muetra versión corta:

    git log --oneline

Muestra una cantidad de commit seleccionado

    git log - <cantidad/numero> 
    
    git log -2

Busco por fechas

    git log --since="2022-02-01"
    git log --after="2022-07-02"
    git log --before="2022-03-04"

Hasta se pueden convinar

    git log --since="<fecha>" --before="<fecha>" --online -4


## GITIGNORE

Archivo que nos permite no darle seguimiento a otros

    .gitignore


## GIT COMMIT

    git commit --help


### Sacar una foto o hacer commit. se abre el editor que hayan configurado

    git commit


### Para poner un mensaje directamente en consola

git commit -m "mensaje"


### Si quiero hacer directamente un git add y un git comit

**IMPORTANTE**: El archivo tiene que estar dentro del repositorio de git. O sea los archivos que estan UNTRACKED no los agrega a la foto.

    git commit -am "mensaje"

### Crear un commit vacío

    git commit --allow-empty -m "mensaje"

### Agregar algo que me olvide

    git commit --amend