# Bandit Walkthrough

## Bandit 16

La contraseña para el siguiente nivel se puede recuperar enviando la contraseña del nivel actual al puerto 30001 en localhost utilizando cifrado SSL/TLS.

Lista de comandos:

```bash
##Entramos al puerto por el servicio ssl
openssl s_client -connect localhost:30001
##Enviamos la contraseña del nivel 15
read R BLOCK
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo


```
Contraseña: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

