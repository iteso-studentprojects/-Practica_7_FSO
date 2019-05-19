# Practica_8_FSO
Práctica 7 de Fundamentos de sistemas operativos. Sistema de archivos 

## Pasos a seguir


Crea el disco virtual 0
	./createvd 0

Crea las particiones del disco virtual 0
	./vdfdisk 0

Da formato a la partición del disco virtual
	./vdformat 0

## Funciones a modificar

Crear procedimiento de funcion vdread
-> filesapi.c -> vdread

```
int vdread(int fd, char *buffer, int bytes)
{
	// Esta es la función a realizar
} 
```

## vdread

Leer datos a partir de donde está el apuntador al archivo previamente abierto
con la función vdopen. A esta función se le debe de indicar como parámetros, el
descriptor del archivo abierto, el buffer donde va a guardar lo que lee del archivo y la
cantidad de bytes a leer.


