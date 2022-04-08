# Comandos basicos de git 
1. `git init`<p>Inicializar con .git el directorio actual</p> 
    `git init <nombreRepo>`<p>inicializar con .git un directorio desde cualquier lugar</p>
2. `git add <file.txt>`<p>Agregamos el archivo especificado a staging</p>
    `git add -A`<p>Añade todos los archivos de nuestro repositorio</p>
    `git add .`<p>Cumple la misma funcion del parametro -A</p>
3. `git commit`<p>Genera un commit</p>
    ### Parametros
    `-a ` <!--Add--><p>Agrega los archivos a staging</p>
    `-m` <!--Message--><p>Añade un mensaje al commit</p>
    `-am`<p>Añade todos los archvios a staging y agrega un mensaje al commit</p>
    `git commit --amend`<p>Permite modificar el ultimo commit,.Antes se debe ejecutar git add</p>
4. `git status`<p>Permite saber el estado de los archivos en el repositorio</p>
5. `git show`<p>Lista de detalles del ultimo objeto de confirmacion</p>
    ### Parametros 
    `git show-branch`<p></p>
    `<archivo>`<p>Para ver los cambios del archivo</p>
6. `git log`<p>Historial de commits de nuestro proyecto</p>
    ### Parametros
    `--stat`<p>Estado de un commit con respecto al anterior</p>
    `--oneline`<p>Muestra en una sola linea cada commit</p>
    `--graph`<p>Muestra el historial de una forma grafica</p>
7. `git diff`<p>Compara dos commits</p>
        <p>Lo que tenga el commit que no tenga el segundo va resaltado en rojo y lo que tenga el segundo que no tenga el primero va resaltado en verde</p>
        `SHA1`<p>Compara el commit indicado(SHA1) con HEAD</p> 
        `SHA2 SHA1`<p>Compara el SHA2 con SHA1</p>
        `SHA1 SHA2`<p>Compara el SHA1 con SHA2</p>
8. `git rm`<p>Eliminar archivos del seguimiento de git</p>
    ### Parametros
    `--cached`<p>Saca el archivo de staging, asi que perdera el seguimiento de git a menos que se ejecute git add</p>
    `--force`<p>Elimina el archivo del disco, en proximas confirmaciones el archivo no estara incluido</p>

9. `git reset`<p></p> 
    ### Parametros
    <p>Todos los commits posteriores al indicado se eliminaran</p>
    `HEAD`<p>Regresa del estado staged a su anterior estado(untracked o unstaged)</p>
        `--hard <hash>`<p>Borra todo el historial commits</p>
        `--soft <hash>`<p>Borra todos los commits pero los cambios los deja en staging</p>
        ### Reiniciar con una ruta <br>
        `git reset "HASH" "file.txt"`<p>El archivo cambia a la version indicada en staging(tambien llamado index)</p>
        <p>Aplastar commits</p>
10. `git reflog`<p>Si por accidente se elimino un commit, al usar git reflog aparecera el historial de git, hacemos git reset --hard SHA y lo traemos de vuelta</p>

11. `git ls-files -s`
12. `rm -rf .git`<p>Eliminar un proyecto inicializado con git</p>
13. `git checkout`<p>Moverse entre ramas y volver a versiones anteriores</p>
    ### Parametros
    `git checkout SHA1 <archivo>`<p>moverse a una version especifica del archivo</p>
    `git checkout master <archivo>`<p></p>
