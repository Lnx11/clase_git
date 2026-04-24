## Desarrollo colaborativo con GitHub.

La diferencia de Git y GitHub es que Git es un sistema de control de versiones, mientras que GitHub es una plataforma en línea que utiliza Git para alojar y gestionar proyectos de software. Git permite a los desarrolladores rastrear cambios en su código, colaborar con otros y mantener un historial de versiones, mientras que GitHub proporciona una interfaz web para facilitar la colaboración, el seguimiento de problemas, la revisión de código y la gestión de proyectos.

Git es app de escritorio, trabaja localmente. GitHub es una plataforma en línea, trabaja en la nube.

A la hora de crear un protecto, se debe crear una carpeta .git, que es donde se guardan los archivos de configuración y el historial de versiones del proyecto. Luego, se pueden agregar archivos al repositorio utilizando el comando `git add`, y luego confirmar los cambios con `git commit`. Para compartir el proyecto en GitHub, se debe crear un repositorio en GitHub y luego vincularlo con el repositorio local utilizando el comando `git remote add origin <URL del repositorio>`. Finalmente, se pueden subir los cambios al repositorio remoto con `git push origin master` (o la rama correspondiente).

`git init` se utiliza para inicializar un nuevo repositorio Git en un directorio existente. Crea una carpeta oculta llamada `.git` que contiene toda la información necesaria para el control de versiones del proyecto.
                |
                V
# Creación de un repositiorio en Git.

configurar por primera vez git con el comando `git config --global user.name "Tu Nombre"` y `git config --global user.email "tu.email@ejemplo.com"`

La carpeta .git no debe borrarse ya que es donde guarda cada version.

si aparece (master) usar en CMD git config --global init.defaultBranch main
luego, borrar carpeta oculta git, y luego volver a iniciar el repositorio con `git init`. Siempre antes de empezar a codear.

git status para saber en que estado estan los archivos. git add para agregar archivos. git commit -m "mensaje" para confirmar los cambios. git push origin main para subir los cambios al repositorio remoto en GitHub. git log --oneline para saber el mensaje de cada commit. git log para saber toda la info completa.
git show y el codigo obtenido de log --oneline para saber que cambios se hicieron en cada commit. git diff para ver que se modifica.
git add . para guardar pequeños pasos en el mismo lugar. De caso contrario se debe guardar completo. Tambien siempre es add/status/commit -m y quizas push la final.

# Status de archivos:
- Untracked: archivos que no están siendo rastreados por Git.
- Unmodified: archivos que están siendo rastreados por Git pero no han sido modificados desde el último commit.
- Modified: archivos que han sido modificados desde el último commit pero aún no han sido confirmados.
- Staged: archivos que han sido modificados y están listos para ser confirmados en el próximo commit.
- Committed: archivos que han sido confirmados en el historial de versiones de Git.



