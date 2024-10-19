# Bandit Walkthrough

## Bandit 22

Un programa se está ejecutando automáticamente a intervalos regulares desde cron, el programador de trabajos basado en el tiempo. Busca en /etc/cron.d/ la configuración y verifica qué comando se está ejecutando.

Lista de comandos:

```bash
##Entramos al directorio y vemos todos los arhcivo al ser pocos
cd /etc/cron.d/
ls
cat *
## Vemos los archivos cronjob_bandit2
cat /usr/bin/cronjob_bandit2*
## Deci que en el archivo esta la contraseña
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

```
Contraseña: tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
