# Bandit Walkthrough

## Bandit 23

Un programa se está ejecutando automáticamente a intervalos regulares desde cron, el programador de trabajos basado en el tiempo.
Busca en `/etc/cron.d/` la configuración y verifica qué comando se está ejecutando.

Lista de comandos:

```bash
##Entramos al directorio
cd /etc/cron.d
##Vemos el archivo de este nivel
cat cronjob_bandit23
##Vemos el archivo cronjob_bandit23.sh
cat cronjob_bandit23.sh
##Declaramos una variable
bandit22@bandit:/etc/cron.d$ myname=bandit23
##Lanzamos el comando incluyendo  la variable previamente declarada
bandit22@bandit:/etc/cron.d$ echo I am user $myname | md5sum | cut -d ' ' -f 1
##Nos da el archivo que contiene la contraseña
cat /tmp/8ca319486bfbbc3663ea0fbe81326349
```
Contraseña: 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
