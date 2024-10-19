# Bandit Walkthrough

## Bandit 21

Hay un binario setuid en el directorio personal que hace lo siguiente: establece una conexión a localhost en el puerto que especificas como argumento de línea de comandos. Luego, lee una línea de texto de la conexión y la compara con la contraseña del nivel anterior (bandit20). Si la contraseña es correcta, transmitirá la contraseña para el siguiente nivel (bandit21).

Lista de comandos:

```bash
##Vemos los puertos abiertos y analizamos a cual nos conectamos
nmap localhost
##Enviamos la contraseña por el puerto 1234
bandit20@bandit:~$ echo -n "0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO" | netcat -lp 1234 &
##Nos conectamos al puerto 1234 y nos da la nueva contresaña
bandit20@bandit:~$ ./suconnect 1234

```
Contraseña: EeoULMCra2q0dSkYj561DX7s1CpBuOBt
