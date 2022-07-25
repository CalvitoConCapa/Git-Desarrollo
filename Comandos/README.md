# Alias

## Para crear un comando

    git config --global alias.
    
    EJ: git config --global alias.l "log --online"

* Despue del "alias." indicar una letra o numero para el comando
* Luego entre comillas, la acción a hacer


## Para ver los comandos echos 

    git config --get-regexp alias


## Para borrar un alias

git config --global --unset alias.
EJ: git config --global --unset alias.s


## Ver alias disponibles

git config --get-regexp alias

# Comandos

* l = git log --oneline
* s = git status --s / status --short 
* c = git commit -m