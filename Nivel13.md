# Bandit Walkthrough

## Bandit 13

La contraseña para el siguiente nivel está almacenada en el archivo data.txt, que es un volcado hexadecimal (hexdump) de un archivo que ha sido comprimido repetidamente. Para este nivel, puede ser útil crear un directorio en /tmp en el que puedas trabajar. Usa mkdir con un nombre de directorio difícil de adivinar. O mejor aún, usa el comando “mktemp -d”. Luego, copia el archivo de datos usando cp, y cámbiale el nombre usando mv (¡lee las páginas del manual!).

Lista de comandos:

```bash
## Entramos en la carpeta temporal
cd /tmp

## Creamos un directorio
mkdir juanmaklk

## Nos movemos al nuevo directorio
cd juanmaklk

## Copiamos el archivo data.txt desde el home
cp ~/data.txt ./

## Convertimos el hexdump a binario y guardamos como data.bin
xxd -r data.txt > data.bin

## Renombramos el archivo binario a data.gz para indicar que es un archivo gzip
mv data.bin data.gz

## Descomprimimos el archivo gzip
gunzip data.gz

## Verificamos el tipo de archivo resultante después de descomprimir
file data

## Extraemos el contenido del archivo tar
tar -xvf data

## Verificamos el tipo del archivo extraído data5.bin
file data5.bin

## Extraemos el archivo data5.bin si es otro tar
tar -xf data5.bin

## Verificamos el tipo del archivo extraído data6.bin.out
file data6.bin.out

## Extraemos el archivo data6.bin.out si es otro tar
tar -xf data6.bin.out

## Verificamos el tipo del archivo extraído data8.bin
file data8.bin

## Renombramos el archivo data8.bin a data8.gz, asumiendo que es un archivo gzip
mv data8.bin data8.gz

## Descomprimimos el archivo gzip data8.gz
gunzip data8.gz

## Verificamos el tipo del archivo final data8
file data8

## Mostramos el contenido del archivo data8
cat data8


```
Contraseña: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

