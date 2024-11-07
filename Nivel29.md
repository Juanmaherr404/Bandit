# Bandit Walkthrough

## Bandit 29

Hay un repositorio git en ssh://bandit28-git@localhost/home/bandit28-git/repo a través del puerto 2220. La contraseña para el usuario bandit28-git es la misma que para el usuario bandit28.

Lista de comandos:

```bash
##Entramos al directorio
mkdir -p /tmp/juanma

##Clonamos un repositorio en esa carpeta
git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo


$ cat ./repo/README.md 

# Vemos el contenido del archivo
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx

## Hacemos un git log para comprobar que commit se han hecho antes
git log
commit 817e303aa6c2b207ea043c7bba1bb7575dc4ea73 (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Thu Sep 19 07:08:39 2024 +0000

    fix info leak

commit 3621de89d8eac9d3b64302bfb2dc67e9a566decd
Author: Morla Porla <morla@overthewire.org>
Date:   Thu Sep 19 07:08:39 2024 +0000

    add missing data

commit 0622b73250502618babac3d174724bb303c32182
Author: Ben Dover <noone@overthewire.org>
Date:   Thu Sep 19 07:08:39 2024 +0000

    initial commit of README.md

## Ahora vamos a hacer un checkout del commit anterior
$ git checkout 3621de89d8eac9d3b64302bfb2dc67e9a566decd

## Vemos el contenido del archivo
cat ./repo/README.md 

# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7

```
Contraseña: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7
