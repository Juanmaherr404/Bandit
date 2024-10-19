# Bandit Walkthrough

## Bandit 7

La contraseña para el siguiente nivel está almacenada en algún lugar del servidor y tiene todas las siguientes propiedades:

- Propietario del usuario bandit7
- Propietario del grupo bandit6
- 33 bytes de tamaño

Lista de comandos:

```bash
##Buscamos un archivo con la descripcion que nos dan
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
##Accedemos al archivo
cat /var/lib/dpkg/info/bandit7.password

```
Contraseña: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
