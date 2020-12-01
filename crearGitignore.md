### Crear archivo .gitignore

Cuando hacemos git add. preparamos todos los archivos que hayan sido modificados. Pero muy a menudo hay archivos en el directorio de trabajo que no queremos que se añadan. Para evitar este problema y facilitar el trabajo, git permite crear un archivo donde escribir qué archivos se quieren ignorar.
El archivo debe llamase ".gitignore" (comenzando por punto) y ubicarse en el directorio raíz del proyecto.
En este archivo se deben incluir los nombres de archivos que se quieran ignorar.
Cada repositorio puede tener su propio .gitignore, pero es útil tener además un archivo general para todos los repositorios.