# Bandit Walkthrough

## Bandit 28

Hay un repositorio de Git en ssh://bandit27-git@localhost/home/bandit27-git/repo a través del puerto 2220. La contraseña para el usuario bandit27-git es la misma que la del usuario bandit27.

Lista de comandos:

```bash
##Lo primero que debemos hacer es crear un carpeta tmp
mkdir -p /tmp/juanma
cd /tmp/juanma

##Clonamos un repositorio en esa carpeta
git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo

##Accedemos al archivo README del repositorio
cat ./repo/README 
The password to the next level is: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

```
Contraseña: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN
