# Bandit Walkthrough

## Bandit 10

La contraseña para el siguiente nivel está almacenada en el archivo data.txt en una de las pocas cadenas legibles por humanos, precedida por varios caracteres ‘=’.

El comando:

```bash
##Accedemos al archivo y ponemos el comando strings para ver el contenido y como la contraseña esta precedida por varios caracteres '='

strings ./data.txt | grep "=="

```
Contraseña: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
