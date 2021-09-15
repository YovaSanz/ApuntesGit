# Comando de Git

## Configuracion
    git --version                                           <!--Muestra la version-->
    git config --global user.name "YovaSanz"                <!--Agregar un usuario globalmente-->
    git config --global user.name                           <!--Ver el usuario>
    git config --global user.email "email@email.com"        <!--Agregar un email/Correo globalmente-->
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

## Hacer Commit
    git commit
    git commit -m "Mensage"

## Ver Commits
    git log
