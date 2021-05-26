# Git
Comandos en Github  :octocat:

Iniciar un proyecto de git odeterminar la carpeta en la que vamos a trabajar.
```
git init  
```

Saber si tenemos un archivo añadido o borrado en nuestro proyecto, para saber en la rama en la que estamos y si tenemos commits.
```
git status
```

Añadir un archivo a nuestra rama seguidamente ponemos entre comillas el nombre de nuestro archivo o poner un punto para añadir todos los archios de nuestra carpeta.
```
git add
```

Borrar un archivo que hayamos añadido, para eliminarlo por completo de nuestra rama usamosgit rm --cached.
```
git rm
```

Añadir un commit a nuestra rama, también podemos ponerle un -m seguidamente ponemos entre comillas nuestro ensaje.
```
git commit
```

muestra configuraciones de git también podemos usar **–list** para mostrar la configuración por defecto de nuestro git y si añadimos **--show-origin inhales** nos muestra las configuraciones guardadas y su ubicación.
```
git config
```

Cambia de manera global el nombre del usuario, seguidamente ponemos entre comillas nuestro nombre.
```
git config --global user.name
```

Cambia de manera global el email del usuario, seguidamente ponemos entre comillas nuestro nombre.
```
git config --global user.email
```

Para ver la historia de nuestros archivos, los commits, el usuario que lo cambió, cuando se realizaron los cambios etc. seguidamente ponemos el nombre de nuestro archivo.
```
git log
```
