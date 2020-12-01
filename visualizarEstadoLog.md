
### Visualizar estado log

Después de haber hecho uno o varios commits, o si has clonado un repositorio que ya tenía un histórico de commits, probablemente el usuario quiera mirar atrás para ver los commits que se han llevado a cabo. Esto es posible con el comando:

```sh
git log
```

Para este comando existen diferentes opciones para su visualización. A continuación se exponen las opciones más comunes:

###### Logs en una sóla línea

Muestra el historial de commits reducidos a una sóla línea para una mejor visualización:

```sh
git log --oneline
```

###### Mostrar todos los commits

Si el usuario desea visualizar todos los commits hasta ese momento, la opción que debe usar en git log es:

```sh
git log --all
```

###### Diagrama de ramas

Si el repositorio tiene ramas (branchs) existe la opción de mostrar más información de las ramas existentes y sus uniones (merges) con la opción siguiente:

```sh
git log --graph
```

Dicho comando se puede combinar con --oneline:

```sh
git log --graph --oneline
```

Y con --decorate, para una mejor visualización:

```sh
git log --graph --oneline --decorate
```

###### Mostrar "n" commits

Si el usuario desea visualizar los "n" últimos commits puede añadir "-n" con el número de commits que desea visualizar (1, 2, 3, 4 ... etc). La opción quedaría de la siguiente forma:

```sh
git log -n
```
