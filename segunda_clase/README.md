## Segunda clase de git

# Git ignore:
    me permite indicar los archivos o carpetas que quiero que no formen parte del repositorio. Ejem.: Archivos de log durante el desarrollo, archivos temporales, etc. Para crear un archivo .gitignore, simplemente se debe crear un archivo de texto con ese nombre en la raíz del proyecto y luego agregar las rutas o patrones de los archivos o carpetas que se desean ignorar. Por ejemplo, si quiero ignorar todos los archivos con extensión .log, puedo agregar la línea `*.log` al archivo .gitignore.

con --short en status puedo ver mas sencillo que esta en espera a ser subido

se crea el archivo .gitignore dentro de la raíz del proyecto, y se agregan las rutas o patrones de los archivos o carpetas que se desean ignorar. Por ejemplo, si quiero ignorar todos los archivos con extensión .log, puedo agregar la línea `*.log` al archivo .gitignore.

git branch -av para saber como esta actualizado.
git log --oneline para ver el historial de commits de forma resumida.

# .gitkeep
Ayuda a git a versionar carpetas que queiro que sean parte del repo, pero estan vacias. Creado por la comunidad, no es un archivo oficial de git. Se crea un archivo vacío llamado .gitkeep dentro de la carpeta vacía que se desea versionar. De esta manera, git reconocerá la carpeta y la incluirá en el repositorio, incluso si no contiene ningún archivo.

# branches o ramas:

las ramas permiten trabajar en diferentes versiones del proyecto de forma simultánea. La rama principal se llama "main" o "master", y es la rama donde se encuentra la versión estable del proyecto. Las ramas secundarias se crean a partir de la rama principal para desarrollar nuevas funcionalidades, corregir errores o experimentar sin afectar la versión estable. Una vez que el trabajo en una rama secundaria está completo, se puede fusionar (merge) con la rama principal para integrar los cambios realizados.

### Listar ramas:
    git branch. locales
    git branch -r. remotas
    git branch -av. ambas

para agragar descripcion de commits, se puede usar git commit solo. ctrl + o para guardar y ctrl + x para salir del editor de texto.

procedimiento: git add + archivo. git commit. ctrl + o + enter para guardar. ctrl + x para salir.


### Creando ramas:
    git branch > feature/rama_nueva. crea la rama pero no cambia a ella.
    git switch -c feature/nombre_rama. crea y cambia a la nueva rama.

    git branch -av para ver donde estamos parados.
    git log para ver que rama estoy.
    para salir de ramas, git switch main. para volver a la rama principal.

    lo demas funciona igual en cuanto a guardar cambios, hacer commit, etc.

    Fast/forward merge: es un tipo de fusión que ocurre cuando la rama de destino no ha tenido ningún cambio desde que se creó la rama de origen. En este caso, git simplemente mueve el puntero de la rama de destino hacia adelante para incluir los cambios de la rama de origen, sin necesidad de crear un nuevo commit de fusión.
    git merge feature/ramas. para fusionar la rama secundaria con la rama principal. Si no hay conflictos, se realizará un fast/forward merge automáticamente. Si hay conflictos, git indicará que se deben resolver antes de completar la fusión.
