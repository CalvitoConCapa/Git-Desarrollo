# GIT DESARROLLO COLABORATIVO

## Markdown
Sistema de etiquetado en HTML

# h1
## h2
### h3
#### h4
##### h5
###### h6
<h1>holaa</h1>

**Soy un texto en negritas**
*Soy un texto en cursiva*

## listas
1. hola
2. hola
3. hola

* Item
* Item
* Item

# COMANDOS CONSOLA

* ls - listar directorios
* cd - cambiar directorios
* cd <directorio> (entra al directorio)
* cd.. (sale del directorio, win= cd../linux= cd ..)
* clear - limpia consola
* mkdir - crea directorios
* touch - crea archivos vacios
* rm - borra archivos

# VERIFICAR QUE TENGO GIT

    git --version

# INCLUIR SNIPPETS

```sh
    git --version
```

```js
    function sumar (a +b){
        return = a + b
    }
```

# Configuro GIT

git config --global user.name "<Nombre>"
git config --global user.email "<Email>"

# Configuro GIT por repositorio

git config --local user.name "<Nombre>"
git config --local user.email "<Email>"

### Para ver el estado del Working directory

    git status
    git status -s (Lo mismo pero sin las ayudas(MEGA-RESUMEN))

### Para subir al escenario los archivos (Staging Area)

    git add <nombre>
    git add . # Agrega todos los archivos al escenario

### Para sacar la foto (Hacer un commit)

    git commit -m "<mensaje>"

### Para agregar un repositorio remoto a mi repo local

    git remote add origin <url>

### Para suber el repositorio local a remoto

    git push -u <remoto> <local>
    git push -u origin master