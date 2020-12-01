### Ayuda detallada sobre git

```sh 
$ git –help
```

### Ayuda detallada sobre un comando concreto

```sh 
$ git --help nombreComando
```

### Opciones de configuración

```sh 
$ git config –list
```

### Agregar nombre de usuario

```sh 
$ git config --global  user.name
```

### Agregar email usuario

```sh 
$ git config --global user.email
```

### Configurar un alias

```sh 
$ git config --global alias.nombreDelAlias
```

### Ver los alias que tenemos y agregar más

```sh 
$ git config --global –e
```

### Hacer que la interfaz use colores para resaltar distintos aspectos en el texto

```sh 
$ git config --global color.ui true
```

### Cambiar la ubicación del archivo .gitignore

```sh 
$ git config --global core.excludesfile rutaAlArchivoIgnore
```