# Git
Comandos útiles en Github  :octocat:

Iniciar un proyecto de git o determinar la carpeta en la que vamos a trabajar.
```
git init  
```

Cambia de manera global el nombre del usuario, seguidamente ponemos entre comillas nuestro nombre.
```
git config --global user.name
```

Cambia de manera global el email del usuario, seguidamente ponemos entre comillas nuestro nombre.
```
git config --global user.email
```

Saber si tenemos un archivo añadido o borrado en nuestro proyecto, para saber en la rama en la que estamos y si tenemos commits.
```
git status
```

Añadir un archivo a nuestra rama seguidamente ponemos entre comillas el nombre de nuestro archivo o poner un punto para añadir todos los archios de nuestra carpeta.
```
git add archivo.jsx
git add .
```

Borrar un archivo que hayamos añadido, para eliminarlo por completo de nuestra RAM usamos **git rm --cached** o bien puedes remover un solo archivo adjuntando el nombre del mismo y su extencion
```
git rm archivo.jsx
git rm --cached
```

Añadir un commit a nuestra rama, también podemos ponerle un **-m** seguidamente ponemos entre comillas un mensaje que represente el commit.
```
git commit -m "Mensaje que represente el commit"
```

Muestra configuraciones de git también podemos usar **-–list** para mostrar la configuración por defecto de nuestro git y si añadimos **--show-origin inhales** nos muestra las configuraciones guardadas y su ubicación.
```
git config
git config -–list
git config -–list --show-origin inhales
```

Para ver la historia de nuestros archivos, los commits, el usuario que lo cambió, cuando se realizaron los cambios etc. seguidamente ponemos el nombre de nuestro archivo.
```
git log
```
