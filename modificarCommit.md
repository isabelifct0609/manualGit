### MODIFICAR COMMIT

El comando git commit --amend es una forma práctica de cambiar la confirmación más reciente. Esto le permite combinar los cambios en el nivel de ensayo con la confirmación anterior en lugar de crear una confirmación completamente nueva. También puede usar este comando para simplemente editar el mensaje de confirmación anterior sin cambiar la instantánea correspondiente. Sin embargo, la corrección no solo cambia la confirmación más reciente, sino que la reemplaza por completo. Esto significa que la confirmación corregida representa una nueva unidad con su propia referencia. Git lo trata como una confirmación completamente nueva, que se puede reconocer con el asterisco (*) en el diagrama a continuación. Hay algunos escenarios comunes para usar git commit --amend. 

```sh
$ git commit --amend
```
