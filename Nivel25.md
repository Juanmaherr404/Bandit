# Bandit Walkthrough

## Bandit 25

Un daemon (proceso en segundo plano) está escuchando en el puerto 30002 y te dará la contraseña para el nivel bandit25 si le das la contraseña de bandit24 y un código PIN numérico secreto de 4 dígitos. No hay manera de obtener el código PIN excepto probando todas las 10,000 combinaciones posibles, lo que se conoce como fuerza bruta. No es necesario crear nuevas conexiones cada vez.

Lista de comandos:

```bash
##Hacemos un bucle for para probar todas las combinaciones posibles de 4 digitos mientras nos conectamos al puerto 30002
for i in {0000..9999}; do echo gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 $i; done | nc localhost 30002

```
Contraseña: iCi86ttT4KSNe1armKiwbQNmB3YJP3q4
