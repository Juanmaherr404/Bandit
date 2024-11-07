# Bandit Walkthrough

## Bandit 30

Hay un repositorio Git en ssh://bandit29-git@localhost/home/bandit29-git/repo a través del puerto 2220. La contraseña para el usuario bandit29-git es la misma que para el usuario bandit29.

Lista de comandos:

```bash
##Creamos un carpeta temporal
mkdir -p /tmp/juanma3
cd /tmp/juanma3

##Clonamos el repositorio
git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo

##Entramos al repo
cd repo

##Vemos las ramas que tiene el repo
git branch -a

## Ahora vamos a hacer un checkout a la rama dev
git checkout remotes/origin/dev

###Vemos el contenido del archivo
cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

```
Contraseña: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL
