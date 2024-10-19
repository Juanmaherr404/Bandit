# Bandit Walkthrough

## Bandit 19

La contraseña para el siguiente nivel está almacenada en un archivo llamado "readme" en el directorio personal. Desafortunadamente, alguien ha modificado el archivo .bashrc para cerrarte la sesión cuando inicias sesión por SSH.

Lista de comandos:


```bash
##Entramos por ssh 
ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/sh"
##Entramos al directorio
$ cat readme

```
Contraseña: cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
