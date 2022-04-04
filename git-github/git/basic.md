# Comandos basicos de git 
1. `git init`<p>Inicializar repositorio</p> 
2. `git add <file.txt>`<p>Staged</p>
3. `git commit`<p>Tracked</p>
    ### Parametros
    `-a ` <!--Add--><p></p>
    `-m` <!--Message--><p></p>
4. `git status`<p></p>
5. `git show`<p></p>
6. `git log`<p></p>
    `--stat`<p></p>
7. `git diff`<p></p>

8. `git rm`<p></p>
    ### Parametros
    `--cached`<p></p>
    `--force`<p></p>

9. `git reset`<p></p>
    ### Parametros
    `HEAD`<p></p>
        `--hard`<p></p>
        `--soft`<p></p>
        ### Reiniciar con una ruta <br>
        `git reset "HASH" "file.txt"`<p>El archivo cambia a la version indicada en staging(tambien llamado index)</p>
        <p>Aplastar commits</p>

10. `git checkout <rama_hash>`<p></p>
    ### Parametros
    `-b`<p></p>

11. `git merge <rama>`
12. `git branch`
    ### Parametros
    `-d`<p></p>
    `-D`<p></p>
    `-M <nueva_rama>`<p></p>
     
12. `git checkout`
13. `git ls-files -s`