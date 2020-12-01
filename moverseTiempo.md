### Moverse en el tiempo

En Git existe una herramienta compleja y versátil para deshacer cambios, muy útil al igual que peligrosa, es por ello que hay que tener cuidado a la hora de usarla. Dicha herramienta moverá el puntero HEAD y el de referencia al momento que el usuario desee. Esto es posible con el comando:

```sh
git reset HEAD [hash]
```

La invocación predeterminada de *git reset* tiene argumentos implícitos de *--mixed* y *HEAD*. Esto significa que ejecutar git reset es equivalente a ejecutar *git reset --mixed HEAD*. De esta forma, *HEAD* es la confirmación especificada. En vez de *HEAD*, se puede usar cualquier hash de confirmación SHA-1 de Git.

Para este comando existen diferentes opciones para su visualización. A continuación se exponen las opciones más comunes:

###### --hard

Esta es la opción más directa, PELIGROSA y que se usa más frecuentemente. Cuando se pasa *--hard*, los punteros de referencia del historial de confirmaciones se actualizan a la confirmación especificada. A continuación, el índice del entorno de ensayo y el directorio de trabajo se restablecen para reflejar la confirmación especificada. Todos los cambios pendientes anteriores del índice del entorno de ensayo y el directorio de trabajo se restablecen para reflejar el estado del árbol de confirmaciones. Esto significa que se perderá cualquier trabajo pendiente que estuviera colgado en el índice del entorno de ensayo y el directorio de trabajo. La opción quedaría de esta forma: 

```sh
git reset --hard HEAD [hash]
```

###### --mixed

Este es el modo de funcionamiento predeterminado. Se actualizan los punteros de referencia. El índice del entorno de ensayo se restablece al estado de la confirmación especificada. Todos los cambios que se hayan deshecho en el índice del entorno de ensayo se mueven al directorio de trabajo.

```sh
git reset --mixed HEAD [hash]
```

###### --soft

Cuando se pasa el argumento --soft, se actualizan los punteros de referencia y el restablecimiento se detiene ahí. El índice del entorno de ensayo y el directorio de trabajo permanecen intactos.

```sh
git reset --soft HEAD [hash]
```
