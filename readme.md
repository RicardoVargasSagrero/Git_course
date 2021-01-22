Comandos de git más utlizados

# git rm
**git rm --cached**: elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro 

**git rm --force**: Elimina los archivos de git y del disco duro. Git siempre guarda todo, de modo que podremos recuperarlos si es necesario (oero debemos ysar comandos más avanzaos)

# git reset
Este comando es muy peligroso y debemos usarlo solo en caso de emergencia. Recuerda que debemos usar alguna de estas dos opciones:

Hay dos formas de usar git reset: con el argumento --hard, borrando toda la información que tengamos en el área de staging (y perdiendo todo para siempre). O, un poco más seguro, con el argumento --soft, que mantiene allí los archivos del área de staging para que podamos aplicar nuestros últimos cambios pero desde un commit anterior.

**git reset --soft**: Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging, así podemos aplicar las últimas actualizaciones a un nuevo commit.

**git reset --hard**: Borra todo. Todo todito, absolutamente todo. Toda la información de los commits y del área de staging se borra del historial.

**git reset --HEAD**: Este es el comando para sacar archivos del área de Staging. No para borrarlos ni nada de eso, solo para que los últimos cambios de estos archivos no se envién al útlimo commit, a menos que cambiemos de opnición y los incluyamos de nuevo en el staging con _git add_, por supuesto. 

# Creación de ramas 
**git branch <branch_name>**: Crea una nueva rama al respositorio 

**git checkout <branch_name>**: Cambiamos de rama

**git log**: Muestra el historias de cambios realizados en el proyecto

**git show**: Muestra los últimos cambios realizados en el repositorio

# Conexión a Github con SSH
A continuación se muestran algunos comando de ayuda para realizar la conexión a GitHub con SSH.

**git remote -v**: Enlista los origenes del repositorio

 **git remote set-url origin <SSH_remote>**: Conexión por ssh a GitHub 

# Tags y versiones en Git y GitHub
**git log**: Muestra el log de cambios realizados en el repositorio

**git log --all --graph**: Muestra el log con sus ramas de forma grafica

**git log --all --graph --decorate --oneline**: Muestra una versión gráfica reducida de las ramas y commits del repositorio

**git tag -a <version del proyecto> -m "<Mensaje del tag>" <hash del commit>**: realiza un tag a un commit del repositorio, esto nos sirve para saber que versión es la estable hasta el momento

# Linux command alias 
 
El comando *alias* crea un alias para un comando largo, por ejemplo para crear un _alias_ para el comando "git log --all --graph --decorate --oneline" se realiza de la siguiente forma

* alias arbol="git log --all --graph --decorate --oneline"