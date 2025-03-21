# Git

Git fue creado pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente, es decir Git nos proporciona las herramientas para desarrollar un trabajo en equipo de manera inteligente y rápida y por trabajo nos referimos a algún software o página que implique código el cual necesitemos hacerlo con un grupo de personas.

# Aprende a Usar Git
Vamos a conocer los comandos principales de Git por medio de una práctica en la que trataremos de ilustrar cuál es el uso de la 
herramienta para gestionar las versiones de un proyecto. El objetivo es ver cómo se crea un repositorio, cómo se actualizan los archivos 
del repositorio y cómo podemos volver hacia atrás para recuperar el estado de los ficheros en versiones anteriores de desarrollo.
Posteriormente, veremos cómo se puede crear en Github un repositorio y cómo podemos mandar los cambios de nuestro repositorio Git en local 
a Github.
## Instalando Git
Es muy fácil de instalar, obteniendo la descarga desde su página oficial:
http://git-scm.com/

En Windows la descarga es un ejecutable que puedes instalar normalmente. En Mac también puedes instalarlo a través del archivo que 
descargas, así como bajarlo usando Home Brew. En Linux lo encuentras en todos los repositorios de las principales distribuciones, cuyos 
paquetes instalas con Apt­get, Yum, etc.

No tenemos que asustarnos por usar la consola de comandos, pero si lo deseamos podemos usar herramientas visuales, que hay un montón, así 
como también se puede integrar Git en la mayoría de los IDE e incluso por medio de plugins en editores de código como Sublime Text.

## Creando un repositorio en local
Es tan sencillo como irse a un directorio de nuestra máquina desde la línea de comandos o desde Git Bash, si estás en Windows. Empezamos 
con un directorio vacío, ya que se supone que estamos comenzando nuestro proyecto y entonces podemos lanzar el comando:
git init

A partir de ese momento tienes todo un repositorio de software completo en tu máquina del proyecto que tenías en ese directorio. Puedes 
crear los archivos que quieras en el directorio (tu proyecto) y luego puedes enviarlos al repositorio haciendo un "commit".
Añadir ficheros al repositorio
Antes de enviar cambios al repositorio, lo que se conoce como hacer commit, tienes que enviar los ficheros a un área intermedia llamada "staging area" en donde se almacenan los archivos que serían actualizados en el próximo commit. Éste es uno de los conceptos esenciales para aprender Git y para mandar los ficheros a este área tenemos que añadirlos al repositorio.
git add

Con ese comando paso los ficheros al "staging area" y a partir de ahí podremos hacer el commit sobre esos ficheros.

git commit ­m "este es mi primer commit"

Ese comando permite enviar los archivos a una especie de base de datos donde puedes colocar los archivos cuyo estado queremos siempre memorizar.

Aquí en el vídeo hablamos brevemente de las ramas y de cómo se gestionan en Git y mencionamos que la rama principal, que se crea al iniciarse el repositorio; se llama "master". También vemos cómo localizar los commits a través de su identificador, lo que nos sirve para poder movernos entre las actualizaciones de software.

Cada vez que se modifica un fichero, se tiene que agregar al área intermedia con el comando "add" y luego hacer el commit para que se actualice el repositorio con los archivos nuevos o actualizados. Eso significa que en teoría cada vez que cambias un archivo tendrías que añadirlo al Staging area para poder hacer el commit, aunque más adelante veremos que hay maneras de automatizar las tareas un poco más y, mediante atajos, poder resumir el paso de hacer el "add" cuando se ha cambiado el código de un fichero.

Deshacer cambios
En cualquier momento puedo deshacer cambios que haya realizado en los archivos, recuperando versiones anteriores que podamos tener en el repositorio. Podría descartar los cambios que tengo en staging area.
git checkout ­­ nombre_fichero

En Git puedes tener código principalmente en tres lugares, el directorio de trabajo, en el Staging area o en una versión que tengas en un commit antiguo de ese repositorio. Existen diferentes comandos para hacer todas estas cosas, dependiendo del lugar de Git donde tengas el código que quieres recuperar. Pero lo verdaderamente útil y potente que tenemos con el control de versiones es poder recuperar archivos realizados commit anteriores, en el último commit, pero también en otros que tengas más antiguos.

Existen muchos comandos para recuperar código anterior como "reset", en el vídeo se ven varios ejemplos, se explican también como fusionar commits y muchas otras cosas interesantes.

## Github
En el vídeo se ve después cómo trabajar con Github, mostrando las posibilidades de este servicio de almacenamiento de repositorios en remoto. Vemos cómo se crea un repositorio en Git y cómo se puede clonar en nuestro sistema local.
Para trabajar con Github tenemos algunas características importantes como las claves de seguridad SSH, que tenemos que generar en local y llevarnos a Github para dar un nivel de seguridad adicional a las actualizaciones contra los repositorios.

En el vídeo se muestra cómo se crea el repositorio en Github y cómo se clona en local por medio del comando "clone". Una vez clonado se muestra cómo se actualizan los archivos en local, se añaden al área intermedia con "add" y se hace el "commit" al repositorio en local. Por último se envían los cambios al servidor remoto con "push".

Todo esto no es un paso inmediato, pero en el vídeo se explica fantásticamente.

Cuando un usuario hace un pull request desde su fork al repositorio original, github crea en el repositorio orignal una referencia a los commits cuya incorporación se ha solicitado. El repositorio original, el que recibe el pull request, guarda estas referencias en refs/pull/*/head. Recordad que las referencias en git no son más que ficheros que contienen hashes a objetos de git. Estos ficheros están en los servidores de github.

## El curso de Git
Todo el material que se ve en el vídeo no es más que la punta del iceberg, es decir, una pequeña muestra de entre todas las enormes posibilidades de Git. Esta clase de una hora seguro que te servirá para dar los primeros pasos con Git, pero hay mucho más detrás de esta herramienta. Hay todavía muchas cosas que ver y conceptos fundamentales como hacer "fork", "pull", "merge", "checkout", "fetch", "branch"...
Todo ese material lo veremos con detalle en el Curso de Git de EscuelaIT, a lo largo de diez horas de clases en directo que se celebrarán durante algo más de una semana. Este vídeo es solo una pequeña muestra de los contenidos que se verán allí con todo detalle.
