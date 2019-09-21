# TP_SO_i2_Framafe

## a) ¿Como actualizo mi repositorio, al estado que esté el repo que hice FORK?
   **1.** Hay que crear una referencia al repositorio original, al cual le puedes poner cualquier nombre, por ejemplo 'upstream',
se usa el comando: ***git remote add [nombre_elegido] [direccion del repositorio]***
   **2.** Hay que traernos las ramas del repositorio: ***git fetch [nombre_elegido]***
   **3.** Irnos a la rama que queremos actualizar, por ejemplo la master: ***git checkout master***
   **4.** Reescribir nuestra rama master con los commits nuevos de la rama master del repositorio original: ***git rebase [nombre_elegido]/master***
   **5.** Por último, actualizamos nuestro fork remoto con (**-f** es para forzar el cambio): ***git push -f origin master***