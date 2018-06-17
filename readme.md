- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

	`git reset --hard HEAD~1`. Para que deshaga el último commit necesitamos el comando git reset HEAD~1 y para que desaparezca el trabajo del working copy hay que añadirle el commando --hard.
	De esta manera lo que había en el working copy se queda vacío.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

	`git reflog` para buscar el hash del commit desecho anteriormente.

	`git reset --hard commit_hash` para rehacer lo desecho en el paso 11.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

	No. Porque la rama styled se creo en el mismo punto que master formando una lista y tiene en común el commit.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

	Si. El contenido del archivo git-nuestro.md es diferente en esas ramas (lineas diferentes). Git puede unir contenido de un mismo archivo pero en este caso no sabe distinguir que código de los dos, que están en las mismas lineas, es el correcto por lo que necesita que el programador se quede con los cambios buenos o con lo mejor de las dos ramas.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

	No. La rama master al hacer merge absorbe el trabajo que tiene la rama styled. Se mueve el puntero al mismo commit que está y ahora todos los commits están disponibles.

- ¿Qué comando o comandos utilizaste en el paso 25?

	`git log --graph --decorate --pretty=oneline`
	
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

	No. Porque la rama title no esta en la misma lista.

- ¿Qué comando o comandos utilizaste en el paso 27?

	`git reset HEAD~1`

- ¿Qué comando o comandos utilizaste en el paso 28?

	`git checkout -- git-nuestro.md`

- ¿Qué comando o comandos utilizaste en el paso 29?

	`git branch -D title`

- ¿Qué comando o comandos utilizaste en el paso 30?

	`git reflog`

	`git reset --hard commit_hash` 


- ¿Qué comando o comandos usaste en el paso 32?

	`git reflog`

	`git checkout commit_hash`

- ¿Qué comando o comandos usaste en el punto 33?

	`git reflog`

	`git reset --hard commit_hash`
