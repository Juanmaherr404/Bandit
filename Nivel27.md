# Bandit Walkthrough

## Bandit 27

¡Buen trabajo obteniendo una shell! ¡Ahora apúrate y consigue la contraseña para **bandit27**!

Lista de comandos:

```bash
##Insertamos la shell como hemos hecho en el nivel anterior
:set shell=/bin/bash
:shell

##Vemos el contenido del archivo
bandit26@bandit:~$ ls
bandit27-do  text.txt

##Utilizamos bandit27-do para ejecutar el comando cat y le pasamos el archivo de texto
bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27


```
Contraseña: upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB
