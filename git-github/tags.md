### Tags 
1. `git tag`<p>Muestra los nombres de los tags de un proyecto</p>
    ### Parametros 
    `-a <"nombre"> <hash>`<p>Se crea un nuevo tag</p>
    `-m <"mensaje">`<p>Se le agrega un mensaje al tag</p>
    `-d <nombre_tag>`<p>Elimina el tag localmente</p>
    `git tag -a <version>`<p></p>
    `git tag -f -a <version> -m <message> HASH`<p>Renombrar un tag, y eliminar el anterior</p>
    `git tag -l`<p>Ver tags de los SHA</p>
2. `git show-ref --tags`<p>Muestra los commits que fueron generados para la creacion de cada uno de los tags</p>

### Remote tags
`git push <remoto> --tags`<p>Enviamos al repositorio remoto los tags de nuestro repositorio local</p>
`git push <remoto>: refs/tag/nombre-del-tag`<p>Eliminamos el tag del repositorio remoto</p>
