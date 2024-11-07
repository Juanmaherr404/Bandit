# Bandit Walkthrough

## Bandit 31

Hay un repositorio Git en ssh://bandit30-git@localhost/home/bandit30-git/repo a través del puerto 2220. La contraseña para el usuario bandit30-git es la misma que para el usuario bandit30.

Lista de comandos:

```bash
##Creamos un carpeta temporal
mkdir -p /tmp/juanma
cd /tmp/juanma

##Clonamos un repositorio en esa carpeta
git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo

##Accedemos al repo
cd repo
##Vemos que archivo tiene oculto el git
git tag

##Mostramos el archivo oculto
git show secret

```
Contraseña: fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy
