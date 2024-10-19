# Bandit Walkthrough

## Bandit 18

Hay 2 archivos en el directorio personal: passwords.old y passwords.new. La contraseña para el siguiente nivel está en passwords.new y es la única línea que ha sido modificada entre passwords.old y passwords.new.

Lista de comandos:

```bash
##Comparamos los archivos y cogemos linea que ha cambiado
diff passwords.new passwords.old 
42c42
< x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
---
> ktfgBvpMzWKR5ENj26IbLGSblgUG9CzB

```
Contraseña: x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
