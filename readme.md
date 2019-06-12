# Índice

[¿Qué comando utilizaste en el paso 11? ¿Por qué?](#pregunta-1)
[¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?](#pregunta-2)
[El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?](#pregunta-3)
[El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?](#pregunta-4)
[El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?](#pregunta-5)
[¿Qué comando o comandos utilizaste en el paso 25?](#pregunta-6)
[El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?](#pregunta-7)
[¿Qué comando o comandos utilizaste en el paso 27?](#pregunta-8)
[¿Qué comando o comandos utilizaste en el paso 28?](#pregunta-9)
[¿Qué comando o comandos utilizaste en el paso 29?](#pregunta-10)
[¿Qué comando o comandos utilizaste en el paso 30?](#pregunta-11)
[¿Qué comando o comandos utilizaste en el paso 32?](#pregunta-12)
[¿Qué comando o comandos utilizaste en el paso 33?](#pregunta-13)

# Pregunta 1
## ¿Qué comando utilizaste en el paso 11? ¿Por qué?

`$ git reset --hard HEAD~1`

1. Con el comando *git reset* nos movemos a nuestros commit ancestros (padres, abuelos... etc).
2. Con el atributo *--hard* modificamos nuestro *working copy* al de nuestro ancestro.
3. Con *HEAD~1* indico que me quiero mover a mi ancestro inmediato, es decir, mi padre.

# Pregunta 2
## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

`$ git reflog`  
`$ git reset --hard bf4e009`

1. El comando *git reflog* para ver el hash corto del historial de commits.
2. El comando *git reset --hard* por lo mismo que en los puntos *1* y *2* del apartado *11*.
3. Con *bf4e009* indico el hash reducido del commit al que me quiero mover.

# Pregunta 3
## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

`$ git merge master`

* No, porque la rama *styled* está más actualizada que la rama *master*, por lo que no se hace el merge.

# Pregunta 4
## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

`$ git checkout styled`  
`$ git merge htmlify`

* Sí, porque el fichero *git-nuestro.md* ha sido modificado en ambas ramas, *styled* y *htmlify* y ambas no son "familia".

# Pregunta 5
## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

`$ git checkout master`  
`$ git merge styled`

* No, porque la rama *styled* es descendiente de *master*, por lo que al hacer el *merge* se actualiza la rama *master*.

# Pregunta 6
## ¿Qué comando o comandos utilizaste en el paso 25?
`$ git log --graph --decorate --pretty=oneline`

# Pregunta 7
## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

* Sí. Porque *title* era una rama hijo de *master*.

# Pregunta 8
## ¿Qué comando o comandos utilizaste en el paso 27?

`$ git reset HEAD~1`

# Pregunta 9
## ¿Qué comando o comandos utilizaste en el paso 28?

`$ git checkout -- git-nuestro.md`

# Pregunta 10
## ¿Qué comando o comandos utilizaste en el paso 29?

`$ git branch -D title`

# Pregunta 11
## ¿Qué comando o comandos utilizaste en el paso 30?

`$ git reflog`  
`$ git reset a2540f6`

# Pregunta 12
## ¿Qué comando o comandos utilizaste en el paso 32?

`$ git reflog`  
`$ git reset c56b438`

# Pregunta 13
## ¿Qué comando o comandos utilizaste en el paso 33?

`$ git reflog`  
`$ git reset 7f8111c`
