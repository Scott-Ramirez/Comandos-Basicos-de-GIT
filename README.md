# Comandos basicos de Git


1. git init                     <!--Inicializar el repositorio -->
2. git add .                    <!--Preparar para la captura -->
3. git reset .                  <!--Para editar antes de guardar despues de haber ejecutado git add-->
4. git commit                   <!--Capturar los archivos del repositorio -->
5. git checkout -- .            <!--Vuelve a recontruir hasta la ultima vez que se guardo -->
6. git log                      <!--Lista el estado de los commit -->
7. git commit --amend           <!--para editar el mensaje del ultimo commit-->
8. git checkout -b rama-heroes  <!--Para crear una nueva rama -->
9. git checkout master          <!--Para cambiar de ramas -->
10. git branch -d rama-heroes   <!--Para eliminar una rama-->
11. git push                    <!--Para enviar todo el contenido a github-->
12. git commit -am              <!--Para acelerar el proceso de guardar cambios-->
13. git clone                   <!--Clona un repositorio existente-->
14. git config                  <!--Establece el nombre del autor, el correo y demas parametros que git utiliza por defecto-->
15. git status                  <!--Enumera todos los archivos que deben ser confirmados-->
16. git diff                    <!--Muestra las diferencias de archivo que aun no se ponen en escena-->
17. git clean                   <!--Elimina los archivos sin seguimiento de la zona de trabajo-->
18. git fetch                   <!--Permite dsecargar una rama de otro respositorio junto con todss sus confirmaciones y archivos asociados-->
19. git merge                   <!--Es una forma eficaz de integrar los cambios de ramas divergentes-->
20. git pull                    <!--Este comando es la version aotomatizada de git fetch descarga una rama de un repositorio remoto  e inmediatamente despues lo fusiona en la rama actual-->
21. git rebase                  <!--Un cambio de base con git rebase permite mover las ramas, lo que ayuda a evitar confirmaciones de fusión innecesarias-->
22. git rebase -i               <!--La marca -i se usa para iniciar una sesión de cambio de base interactivo. Esto ofrece todas las ventajas de un cambio de base normal, pero te da la oportunidad de añadir, editar o eliminar confirmaciones sobre la marcha-->
23. git reflog                  <!--Git realiza el seguimiento de las actualizaciones en el extremo de las ramas mediante un mecanismo llamado registro de referencia o reflog. Esto permite volver a los conjuntos de cambios aunque no se haga referencia a ellos en ninguna rama o etiqueta-->
24. git remote                  <!--Es un comando útil para administrar conexiones remotas. En lugar de pasar la URL completa a los comandos fetch, pull y push, permite usar un atajo más significativo-->
25. git revert                  <!--Permite deshacer una instantánea confirmada. Si descubres una confirmación errónea, revertirla es una forma fácil y segura de eliminarla por completo del código base-->
26. git log --graph             <!--Para ver el historial de forma detallada-->
# RAMA
Una rama representa una línea independiente de desarrollo. Las ramas sirven como una abstracción de los procesos de edición, ensayo y confirmación que se tratan en Principios básicos de Git, el primer módulo de esta serie. Puedes concebirlas como una forma de solicitar un nuevo directorio de trabajo, un nuevo entorno de ensayo y un nuevo historial de proyecto. Las nuevas confirmaciones se registran en el historial de la rama actual, lo que crea una bifurcación en el historial del proyecto.
# FLUJO DE TRABAJO CENTRALIZADO
Una rama representa una línea independiente de desarrollo. Las ramas sirven como una abstracción de los procesos de edición, ensayo y confirmación que se tratan en Principios básicos de Git, el primer módulo de esta serie. Puedes concebirlas como una forma de solicitar un nuevo directorio de trabajo, un nuevo entorno de ensayo y un nuevo historial de proyecto. Las nuevas confirmaciones se registran en el historial de la rama actual, lo que crea una bifurcación en el historial del proyecto.
# FLUJO DE TRABAJO DE RAMA DE FUNCION
El flujo de trabajo de rama de función se basa en el flujo de trabajo centralizado al encapsular las funciones nuevas en ramas específicas. Esto permite usar solicitudes de incorporación de cambios para comentar los cambios antes de integrarlos en el proyecto oficial.
# CREAR UNA BIFURCACION 
En lugar de usar un repositorio de servidor único que haga de código base "central", la bifurcación ofrece a todos los desarrolladores un repositorio de servidor. Esto significa que cada contribuidor no tiene uno, sino dos repositorios de Git: uno privado local y uno público de servidor.
# FLUJO DE TRABAJO DE GITFLOW
El flujo de trabajo de Gitflow optimiza el ciclo de publicación mediante el uso de ramas aisladas para el desarrollo de funciones, la preparación de la publicación y el mantenimiento. Su estricto modelo de ramificación también aporta una estructura muy necesaria para los proyectos más grandes.
# HEAD
Es la forma en la que Git hace referencia a la instantánea actual. Internamente, el comando git checkout simplemente actualiza el HEAD para que apunte a la rama o la confirmación especificada. Cuando apunta a una rama, Git no objeta nada, pero cuando cambias a una confirmación, pasa al estado "detached HEAD".
# HOOK
Es un script que se ejecuta automáticamente cada vez que se produce un evento en particular en un repositorio de Git. Los hooks permiten personalizar el comportamiento interno de Git y desencadenan acciones personalizables en puntos clave del ciclo de vida del desarrollo.
# PULL REQUEST
Las solicitudes de incorporación de cambios son una función que facilita la colaboración entre desarrolladores que usan Bitbucket. Ofrecen una interfaz web intuitiva para debatir los cambios propuestos antes de integrarlos en el proyecto oficial.
# REPOSITORIOS
Conjunto de confirmaciones, ramas y etiquetas para identificar las confirmaciones.
# ETIQUETA
Referencia que suele utilizarse para marcar un punto en concreto en la cadena de confirmación. A diferencia de lo que ocurre con head, el comando commit no actualiza las etiquetas.
# CONTROL DE VERSIONES 
Sistema que registra los cambios en un archivo o conjunto de archivos a lo largo del tiempo para que se puedan recuperar versiones específicas más adelante.
# ARBOL DE TRABAJO 
El árbol de archivos extraídos, que normalmente incluye el contenido del árbol de HEAD commit y cualquier cambio local que hayas hecho, pero que no hayas confirmado aún.