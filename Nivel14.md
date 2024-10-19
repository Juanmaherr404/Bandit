# Bandit Walkthrough

## Bandit 14

Claro, aquí tienes la traducción:

La contraseña para el siguiente nivel está almacenada en /etc/bandit_pass/bandit14 y solo puede ser leída por el usuario bandit14. Para este nivel, no obtienes la siguiente contraseña, sino que recibes una clave SSH privada que se puede usar para iniciar sesión en el siguiente nivel. Nota: localhost es un nombre de host que se refiere a la máquina en la que estás trabajando.

Lista de comandos:

```bash
##Entramos por ssh a bandit14 por medio de la clave privada
ssh -i sshkey.private -p 2220 bandit14@localhost
##Mostarmos el contenido del archivo
cat /etc/bandit_pass/bandit14 

```
Contraseña: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
