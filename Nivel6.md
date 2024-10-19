# Bandit Walkthrough

## Bandit 6

La contraseña para el siguiente nivel está almacenada en un archivo en algún lugar del directorio inhere y tiene todas las siguientes propiedades:

- Legible por humanos
- 1033 bytes de tamaño
- No es ejecutable

Lista de comandos:

```bash
##Entramos al directorio
cd inhere
## Mostramos el archivo que encaga en la descripcion que nos dice
find . -type f -size 1033c
## Accedemos al archivo
cat maybehere07/.file2
```
Contraseña: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
