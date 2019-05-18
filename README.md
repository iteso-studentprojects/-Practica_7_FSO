# Practica_8_FSO
Práctica 7 de Fundamentos de sistemas operativos. Sistema de archivos 

## Funciones a modificar

Crear procedimiento de funcion vdread
-> filesapi.c -> vdread

```
int vdread(int fd, char *buffer, int bytes)
{
	// Esta es la función a realizar
} 
```
Crear procedimiento de delete para eliminar archivos
-> shell.c -> delu -> unlink

unlink se tiene que declarar e implementar en filesapi.c

```
int delu(char *arg1)
{
	unlink(arg1);
}
```

## vdread

Leer datos a partir de donde está el apuntador al archivo previamente abierto
con la función vdopen. A esta función se le debe de indicar como parámetros, el
descriptor del archivo abierto, el buffer donde va a guardar lo que lee del archivo y la
cantidad de bytes a leer.

## delu

Con su subfunción "unlink" es una función del comando delete que sirve para eliminar
archivos que comuenzan con /unix/ y por lo tanto son archivos que estan en el sistema
de archivos de unix
