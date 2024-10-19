# Bandit Walkthrough

## Bandit 12

La contraseña para el siguiente nivel está almacenada en el archivo `data.txt`, donde todas las letras minúsculas (a-z) y mayúsculas (A-Z) han sido rotadas 13 posiciones.

El comando:

```bash
##Entramos al archivo y le aplicamos la rotacion de 13 posiciones
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
Contraseña: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
