# Comandos Basicos de Git

## Configuracion
    git --version                                           <!--Muestra la version-->
    git config --global user.name "YovaSanz"
    git config --global user.name                           <!--Ver el usuario>
    git config --global user.email "email@email.com"
    git config --global user.email                          <!--Ver el email --->

    <!--crea un alias para un comando en este caso el alias es lg y el comando estan en ""(sin "git")-->
    git config --global alias.lg "log --oneline --decorate --all --graph"

    git config --global -e                                  <!--Muestra el archivo de confirguracion-->

## Agregar al Staged
    git add .
    git add index.html
    git add -Z                                              <!--también los borrados--->

## Quitar del Staged
    git rm --cached index.html

## Estado del Staged
    git status

## Hacer Commit
    git commit
    git commit -m "Mensage"

## Ver Commits
    git log

## Recuperar Commits
    git checkout *Hahs
    git checkout master                                     /*El ultimo commit*/

## RESET Commit         /*Vuelve aun commit aterior eliminando los commit hechos despues de este*/
    Reset soft: git reset --soft *Hahs                      Recupera el commit, indicado en el comando, como último sin modificar el proyecto.
    Reset hard: git reset --hard *Hahs                      Recupera el commit, indicado en el comando, como último modificando el proyecto con las características de dicho commit.




# Comandos para Ramas en Git

## Ver Ramas
    git branch

## Crear Ramas
    git branch pruebas

## Cambiar Rama
    git checkout pruebas

## Unir Ramas
    <!--Debemos estan en la rama donde queramos unir todo-->
    git merge pruebas

## Eliminar Rama
    git branch pruebas -D




# Comandos para GitHub

## Clonar un Repocitorio
    git clone <Link del repositorio>

## Subir Repisitorio a GitHub
    git remote add origin <link del repositorio>
    git remote -v
    git push -u origin master 

## comandos que da github al crear un nuevo repositorio
### o crea un nuevo repositorio en la línea de comandos
    echo "# ApuntesGit" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main                                                              <!-- "-M" lo convierte en master (puede ser no necesario)-->
    git remote add origin https://github.com/YovaSanz/ApuntesGit.git
    git push -u origin main

### o enviar un repositorio existente desde la línea de comandos
    git remote add origin https://github.com/YovaSanz/ApuntesGit.git
    git branch -M main                                                              <!-- "-M" lo convierte en master (puede ser no necesario)-->
    git push -u origin main

