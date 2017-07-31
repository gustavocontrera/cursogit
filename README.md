# cursogit
prueba simultanea entre bitbucket y github

Les cuento que ete proyecto es una prueba para la sincronización simultánea entre Bitbucket y Github

1-Primero armo una carpeta dentro de mi carpeta llamada "repositoriosgit", llamada > "proyectos"

-Luego abro un repositorio en Bitbucket y Github con el mismo nombre "proyectos"

-Ahora inicio git en la carpeta local con git.init

-Ahora agrego la primer dirección remota con:
git remote add origin https://gustavocontrera@bitbucket.org/gustavocontrera/proyectos.git

-Ahora la segunda:
git remote set-url --add origin https://github.com/gustavocontrera/proyectos.git

-Por último para que no me pida usuario y clave cada vez que hago push tengo que agregar por única vez.
git config credential.helper store
(luego sólo me puede pedir las credenciales la primera vez)


######(git remote rm second)(Remover un repositorio de nombre second) antes había agregado la dir remota como: 
git remote add second https://github.com/gustavocontrera/cursogit.git / Pero esto no sirve por que cuando hago 
push origin no me lo sube a los dos repositorios
