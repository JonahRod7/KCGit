11/ Deshacer el último commit (perdiendo los cambios realizados en el working 
copy)
**Pregunta:** ¿Qué comando utilizaste en el paso 11? ¿Por qué?
**Respuesta:** Uso el comando `git reset --hard HEAD~1` porque el comando hard 
se encarga de descartar los archivos en el working copy.

12/ Rehacer el último commit (el que acabamos de deshacer)
**P:** ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
**R:** Uso el comando `git reset --hard <hash>`, asi me dirijo al commit 
requerido tras haberlo identificado con el comando `git reflog`.

13/ Hacer un merge con ‘master’ (styled absorbe a master)
**P:** El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
R: Al comprobar mi posición con `git log --graph`, noto que la rama styled tiene 
acceso a la rama master y al hacer un merge no afectaría en nada.

19/ Hacer un merge de “htmlify” en “styled” (styled absorbe a htmlify)
P: El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
R: Sí, causó conflicto ya que en ambas ramas se había modificado el contenido 
del archivo *git-nuestro.md* por tanto se debe solucionar modificando el archivo 
escogiendo el contenido final para añadir y hacer el commit.

21/ Desde “master”, hacer un merge con “styled”
P: El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
R: Al igual que antes, no causa ningún conflicto ya que la rama styled tiene 
acceso a la rama master.

25/ Dibujar el diagrama
P: ¿Qué comando o comandos utilizaste en el paso 25? 
R: `git log --graph`

26/ Hacer un merge “no fast-forward” de “title” en “master” (master absorbe a 
title)
**P:** El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
**R:** Sí, si fuese fast-forward el puntero HEAD y la rama master se moverían al 
commit de la rama title.

27/ Deshacer el merge (sin perder los cambios del working copy)
**P:** ¿Qué comando o comandos utilizaste en el paso 27?
**R:** `git reset HEAD~1`

28/ Descartar los cambios 
**P:** ¿Qué comando o comandos utilizaste en el paso 28?
**R:** `git checkout git-nuestro.md`

29/ Eliminar la rama “title”
**P:** ¿Qué comando o comandos utilizaste en el paso 29?
**R:** `git branch -D title`

30/ Rehacer el merge que hemos deshecho
**P:** ¿Qué comando o comandos utilizaste en el paso 30?
**R:** `git reflog` `git reset <hash>`

32/ Volver al commit inicial cuando se creó el poema
**P:** ¿Qué comando o comandos usaste en el paso 32?
**R:** `git reflog` `git reset <hash>`

33/ Volver al estado final, cuando pusimos título al poema
**P:** ¿Qué comando o comandos usaste en el punto 33?
**R:** `git reflog` `git reset <hash>`
