1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

Abrimos el fichero y añademos el contenido al fichero. nano scene-5.txt

2. Añade scene-5.txt al área de preparación.

git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

git commit -m "Añadido contenido ultimas lineas"


4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

Volvemos a abrir el fichero y modificamos la palabra flames por ballons.
nano scene-5.txt

5. Devuelve el fichero al estado del último commit.

git log --oneline
git resest --mixed codigo del ultimo commit


6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.

Abrimos los dos ficheros con noa y realizamos los cambios.

7. Añade los ficheros al área de preparación usando un único comando git.

git add scene-3.txt scene-7.txt

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.

nano scene-2.txt y borramos una linea.

9. Añade scene-2.txt al área de preparación.

git add scene-2txt

10. Comprueba el estado del repositorio. 

git status

11. Devuelve scene-2.txt al directorio de trabajo.

git reset scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.

git commit -m "Cambia Larry por Laertes"

13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.

buscar commit: git log --oneline
vovler al commit anterior: git reset código ultimo commit 

14. Crea una nueva rama llamada **reinventando_hamlet**

git branch reinventando_hamlet

15. Cámbiate a dicha rama

git checkout reinventando_hamlet

16. Mejora la escena 2 como creas conveniente.

abrinos el fichero scene-2.txt y lo mejoramos

17. Haz un commit con los cambios con un mensaje adecuado.

git commit -m "añadido contenido"

18. Vuelve a la rama master.

git checkout master

19. Elimina la rama **reinventando_halet**

git branch -d reinventando_hamlet

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.

git branch new_branch
modificamos el archivo scene-2.txt
git commit -m "modificacion en scene-2.txt"
git merge master

21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.

estando en el nueva rama modificamos un fichero.
editamos el archivo scene-2.txt y le añadimos un contenido extra en la primera linea.
lo subimos y añadimos el commit.
nos cambiamos a la rama master con git checkout master
hacemos el merger en la rama principal de larama creada anteriormente.
git merge new_branch
al dar el conflicto abrimos el archivo y elegimos la parte que deseamos guardar el conflicto, hacemos commit y ya tendremos el conflicto resuelto.


