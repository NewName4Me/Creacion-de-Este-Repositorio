
# Creación de este repositorio.

En este pequeño repositorio vas a aprender a como utilizar de forma básica herramientas como **Git** y **GitHub**
Con el fin de realizar un **control de versiones adecuado**, aprender a trabajar en ramas y controlar los datos y cambios que suceden en nuestro programa o aplicación

+ [1. Crearnos una cuenta de GitHub](#paso-1-crearnos-una-cuenta-en-github)
+ [2. Descargamos Git](#paso-2-descargamos-git)
+ [3. Crearnos nuestro primer Repositorio](#paso-3-crearnos-nuestro-primer-repositorio)
+ [4. Abrir Git y Vincular Cuenta](#paso-4-abrir-git-y-vincular-cuenta)
+ [5. Vincular nuestro repositorio a la carpeta local](#paso-5-vincular-nuestro-repositorio-a-la-carpeta-local)
+ [6. Realizar los primeros cambios en Nuestro Repositorio](#paso-6-realizar-los-primeros-cambios-a-nuestro-directorio)
+ [7. Visualizar los cambios sucedidos entre Commits](#paso-7-visualizar-cambios-sucedidos-entre-commits)
+ [8. Aprender a trabajar con ramas de forma Básica](#paso-8-aprender-a-trabajar-con-ramas-de-forma-básica)


## *Paso 1*:   Crearnos una cuenta en GitHub
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>
GitHub es una plataforma que permite a los desarrolladores colaborar en proyectos de software utilizando el sistema de control de version de **Git** que veremos posteriormente. Ofrece herramientas para gestionar proyectos, realizar seguimiento de código, colaborar con desarrolladores y alojar repositorios.

<br>

![Foto de mi Perfil de Github](https://github.com/NewName4Me/MediaForReadMe/blob/main/miperfil.png?raw=true)

## *Paso 2*: Descargamos Git
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>
A pesar de que podamos confundirla con **GitHub** porque da la sensación que hacen lo mismo hay una gran diferencia : **Git** es el *sistema de control de versiones en sí mismo*, mientras que **GitHub** es una plataforma que *utiliza Git* para alojar y gestionar proyectos de software, facilitando la colaboración y la gestión del desarrollo de software en equipo.

<br>

![Foto de mi Perfil de Github](https://github.com/NewName4Me/MediaForReadMe/blob/main/git.png?raw=true)

## *Paso 3*: Crearnos nuestro primer Repositorio
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

+ Vamos a la barra lateral y pulsamos en el apartado de repositorios, que si este es tu primer repositorio debería estar vacío

<br>

![Barra Lateral Git Hub](https://github.com/NewName4Me/MediaForReadMe/blob/main/lateral.png?raw=true)

+ Pulsamos en new para crear nuestro primer repositorio

![Barra Lateral Git Hub](https://github.com/NewName4Me/MediaForReadMe/blob/main/newrepository.png?raw=true)

+ Ahora indicamos el nombre de nuestro proyecto, en mi caso *'Creación de este repositorio'*, e indicamos si queremos que nuestro repositorio sea público o privado, es decir, si queremos que otros usuarios tengan acceso a este. Eso particularmente a nosotros no nos importa dado que nos podemos vincular este repositorio a una carpeta local independientemente de como sea este

![Barra Lateral Git Hub](https://github.com/NewName4Me/MediaForReadMe/blob/main/nombrerepositorio.png?raw=true)

+ Una vez le demos a publicar el propio *GitHub* nos proporcionará los comandos y pasos que debemos seguir para conectar ese repositorio a nuestra carpeta local. Pero como resulta muy confusa e incompleta, por ahora olvidalo y simplemente fijate en la dircción HTTPS que nos propociona, la cual se corresponde con la direccion de este repositorio, es lo único que nos importa.

![Barra Lateral Git Hub](https://github.com/NewName4Me/MediaForReadMe/blob/main/direccionreposirotio.png?raw=true)

## *Paso 4*: Abrir Git y Vincular Cuenta
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

+ Primero de todo creamos una carpeta cualquiera y en ella hacemos click derecho y abrimos *Git* que instalamos anteriormente, este nos va a abrir una terminal que nos concede una sería de comandos únicos que nos permiten el control de versiones

![Foto de la consola en mi carpeta](https://github.com/NewName4Me/MediaForReadMe/blob/main/4.png?raw=true)

+ En esta carpeta es donde vamos a tener localizados los archivos que subiremos a nuestro repositorio, por tanto lo que tenemos que hacer ahora es identicarnos con nuestro nombre de usuario y correo en GitHub, este paso es **totalmente opcional**, en caso de que solo quieras usar *Git* sin *GitHub* puedes saltartelo:

Primero vamos a vincular esta carpeta a la cuenta que tenemos creada en GitHub

Usuario:

    git config --global user.name "tu_nombre_de_usuario"

Correo:

    git config --global user.email "tu_correo_asignado_en_github"

## *Paso 5*: Vincular nuestro repositorio a la carpeta local
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

Primero vamos a crear un archivo *.git*, en esta carpeta, que esta oculta de forma predeterminada, es donde se almacenan los cambios sucedidos en nuestro codigo, para instalarla ejecutamos:

    git init

Ahora, utilizando la direccion HTTPS que guardamos en el paso 3, vamos a vincular nuestro repositorio a nuestro directorio local, para ello vamos a ejecutar en el mismo directorio donde ejectuamos el registro el siguiente comando:

    git remote add origin "URL_Del_Directorio_Remoto"

De esta forma a partir de ahora todos los cambios que hagamos en esta carpeta, podrán verse reflejados en nuestro repositorio siempre y cuando hagamos lo siguiente ⬇️

## *Paso 6*: Realizar los primeros cambios a nuestro directorio
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

+ Vamos a abrir el directorio local en nuestro IDE favorito, por ejemplo VisualStudioCode, una vez aquí creamos un archivo cualquier y lo editamos, yo por ejemplo voy a crear este README.md

![Foto de la consola en mi carpeta](https://github.com/NewName4Me/MediaForReadMe/blob/main/crearReadme.png?raw=true)

+ Si utilizais un editor de código como VisualStudioCode apreciareis unos cambios de color en los archivos además de que aparece la letra U a su lado, eso quiere decir que han sucedido cambios pero no han sido almacenados aún en nuestro .git

Por tanto abrimos la consola de nuevo y ejecutamos el comando:

    git status

Este comando nos muestra si han sucedido cambios en nuestros archivos, nos indica cuales, que debemos cambiar, etc . En caso de que no tengamos un editor de codigo que nos lo muestre al momento.

![Foto del Resultado de hacer git status](https://github.com/NewName4Me/MediaForReadMe/blob/main/gistatus.png?raw=true)

Como podeís ver mi README.md está en rojo, por tanto tenemos que hacer 3 comandos en orden, tres comandos míticos que todos nos debemos aprender : **add, commit, push**

+ **Add** indica que archivos o archivos vamos a guardar 
+ **Commit** nos añade un mensaje a cada uno para identificar la función que tuvieron los cambios realizados y termina de subir el archivo a nuestro directorio *.git*
+ **Push** (opcional si decides no utilizar github), realiza el "despliegue" del último commit a GitHub para que este este al dia

Estos comandos se verían así la primera vez:

    git add README.md
    git commit -m "Creacion del Readme con título"
    git push --set-upstream origin master

**Aclaracion** este último *push* solo se vería así la primera vez que lo ejecutamos, dado que nuestro directorio aún estaba limpio, no teniamos donde subir a nuestro archivo como tal, por tanto a la vez que lo subimos hemos creado la primera **rama**, la rama **master** (más información sobre las ramas siga leyendo), el resto de push que hagamos por ahora se verán así:

    git push

## *Paso 7* Visualizar cambios sucedidos entre Commits
<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

Vamos a entrar a nuestro README.md y vamos a hacer un pocos cambios, por ejemplo una breve introducción.

![Foto del readme actualizado](https://github.com/NewName4Me/MediaForReadMe/blob/main/readme2.png?raw=true)

Vereis que ahora aparece una M, de "modified" es decir se han hecho cambios pero no aparece una U dado que el archivos ya ha sido desplegado.
Por tanto vamos a la consola y ejecutamos nuestros tres comandos

    git add README.md
    git commit -m "añadir una breve introduccion a nuestro repositorio"
    git push

Ahora bien, supongamos que pasa un tiempo, y quieres ver que tenías antes en tu codigo ya sea por comprobar si hiciste algún cambio que no debías, ver la progresión de tu código o tal vez creas que has cometido un error y queiras retroceder.

Para ello, en caso de que nuestro repositorio este en GitHub, podemos hacerlo de forma gráfica muy sencillo, simplemente en nuestro repositorio, despues de la URL escribimos */commit/* (https://github.com/NewName4Me/Creacion-de-Este-Repositorio/commit/) y automaticamente veremos un lista de commits donde se indican los cambios sucedidos entre cada version

![Foto de los commits en GitHub](https://github.com/NewName4Me/MediaForReadMe/blob/main/commitgithub.png?raw=true)


Pero si estamos trabajando con **Git sin GitHub** para ello, primero debemos identificar los commits que queremos comparar, para ello vamos a ver la lista de commits sucedidos utilizando:

    git log

Cuando hagamos esto vemos varias cosas, un código muy largo identificatorio del commit, el autor que lo realizo (uno de los motivos por los que nos logeamos en el Paso 4), fecha, hora y el mensaje que pusimo de commit, por eso es tan importante que nuestro mensaje sea descriptivo.

![Foto de los logs](https://github.com/NewName4Me/MediaForReadMe/blob/main/gitlog.png?raw=true)


Ahora bien, si queremos comparar que cambios se realizaron entre dos commits debemos utilizar los códigos identificativos de estos, de la siguiente manera:

    git diff "codigoDelPrimerCommit1" "codigoDelSegundoCommit2"

Esto nos indicará las diferencias(diff) que hay entre uno y otro.

![Foto de la diferencia](https://github.com/NewName4Me/MediaForReadMe/blob/main/gitdiff.png?raw=true)

Además si en algún momento te arrepientes de algún cambio realizado y quieres **retroceder a un estado previo** una vez con *git log* miras el identificador del commit al que quieres volver y escribes:

    git checkout "nombreDelCommit"

## *Paso 8*: Aprender a trabajar con ramas de forma básica

<div style="text-align: right">
    <a href="#creación-de-este-repositorio">Volver al Índice</a>
</div><br>

Imagina que estás escribiendo un libro y decides explorar diferentes subtramas o ideas para tu historia. Cada una de estas exploraciones la representas con una hoja de papel separada, donde desarrollas y expandes esa idea de forma independiente. Estas hojas de papel son como ramas en Git.

![Foto de persona con un libro escribiendo diferentes paginas](https://github.com/NewName4Me/MediaForReadMe/blob/main/muchasramas.jpeg?raw=true)

Cada vez que te adentras en una nueva subtrama, comienzas una nueva hoja de papel (rama) y trabajas en ella sin afectar la versión principal de tu historia (rama principal o "master"). Puedes hacer cambios, agregar personajes o incluso eliminar escenas en una hoja de papel sin alterar el resto del libro.

Al final, cuando estés satisfecho con una de tus subtramas, puedes integrarla de nuevo en la historia principal (fusionar la rama) para que se convierta en parte de la trama general del libro. De esta manera, las ramas en Git te permiten experimentar, explorar y desarrollar diferentes ideas de manera creativa mientras mantienes la integridad y coherencia de tu proyecto principal.

![Foto de los logs](https://github.com/NewName4Me/MediaForReadMe/blob/main/ramas.png?raw=true)

### *8.1*: Crear Diferentes ramas
**Forma Gráfica (GitHub)**: 
+ Vamos a nuestro repositorio
+ Pulsamos en *master* o la rama que tengamos activa en el momento
+ Pulsamos en *ver todas las ramas*
+ Pulsamos en añadir rama y la nombramos

![Foto de como crear una rama](https://github.com/NewName4Me/MediaForReadMe/blob/main/ramasGitHubt.png?raw=true)

**Por consola** :
Primero nos tenemos que cerciorar de que la rama que vamos a crear no e existe por tanto vamos a ver el listado de ramas existentes con el comando:

    git branch
Además podremos ver en que rama estamos trabajando ahora mismo dado que será la que tiene un '*' al lado

Una vez que sabemos que nombre le podemos poner simplemente ejecutamos

    git branch "nombreQueLeQuierasPoner"

Recuerda que el nombre de la rama tiene que ser identificatorio para los cambios que esta realizando respecto a la principal

### *8.2*: Movernos entre ramas
**Forma Gráfica**:
+ Es tan simple como pulsar en la rama que queremos trabajar y lista, luego podemos descargarnos el repositorio de esa rama pulsando en *Descargar ZIP*

![Foto de como descargar rama](https://github.com/NewName4Me/MediaForReadMe/blob/main/downloadbranch.png?raw=true)

**Por Consola**:

Dado que ya sabemos del paso anterior como podemos averiguar el nombre de la rama a la que nos queremos cambiar

    git branch

Para movernos a una rama cualqueira basta con hacer:

    git checkout "nombreDeLaRamaEnLaQueQueramosTrabajar"

### *8.3*: Publicar una rama

Una vez tenemos una rama creada y nos hemos movido a ella, ya podemos trabajar en esta, hacer los cambios pertinentes y todo lo necesario, incluso realizar comandos como *add, commit* para los cambios que hagamos poco a poco se guarden en *Git*, pero, para que estos cambios sean visibles en *GitHub* antes tenemos que publicar la rama, para ello hacemos:

    git push origin "nombreDeLaRama"

En caso de que lo hubieramos hecho directamente en GitHub ya estaría publicada directamente y esto no es necesario.

### *8.4*: Eliminar ramas

Si creemos que los cambios realizados no son necesarios, y queremos eliminarlos permanentemente junto con todos sus archivos hacemos lo siguiente:

    git branch -d "nombreDeLaRamaAEliminar"

### *8.5*: Renombrar una rama

En caso de que el nombre otorgado a la rama no la identifique correctamente o simplemente queramos cambiar el nombre por cualquier motivo hacemos: 

    git branch -m "nombreActualDeLaRama" "nombreNuevoDeLaRama"

### *8.5*: Combinar ramas con la principal
La rama principal, siempre va a estar ahí, es la rama que dirige la historio de nuestro libro y no la podemos eliminar, por tanto, cuando trabajamos en una rama, la idea es hacer cambios, hasta que estos sean los adecuados para que pueda fusionarso con la rama principal. Para ello nos desplazamos a la rama a fusionar (la que no es la master), y desde ahí hacemos :

    git merge "nombreDeLaRama"

![Foto de Git Work Flow](https://github.com/NewName4Me/MediaForReadMe/blob/main/gitworkflow.jpg?raw=true)