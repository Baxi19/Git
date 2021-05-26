# Git
Comandos útiles en Github  :octocat:

Iniciar un proyecto de git o determinar la carpeta en la que vamos a trabajar.
```
git init  
```

Muestra configuraciones de git también podemos usar **-–list** para mostrar la configuración por defecto de nuestro git y si añadimos **--show-origin** nos muestra las configuraciones guardadas y su ubicación.
```
# todas las configuraciones
git config

# configuracion por defecto de git 
git config -–list

# Para ver donde estan las configuraciones guardadas
git config -–list --show-origin
```

Cambia de manera global el nombre del usuario, seguidamente ponemos entre comillas nuestro nombre.
```
git config --global user.name "Nombre de Usuario"
```

Cambia de manera global el email del usuario, seguidamente ponemos entre comillas nuestro email.
```
git config --global user.email "correo@gmail.com"
```

Saber si tenemos un archivo añadido o borrado en nuestro proyecto, para saber en la rama en la que estamos y si tenemos commits.
```
git status
```

Añadir un archivo a nuestra rama seguidamente ponemos entre comillas el nombre de nuestro archivo o poner un punto para añadir todos los archios de nuestra carpeta.
```
# agregar un archivo especifico
git add archivo.jsx

# agregar todos los archivos
git add .
```

Leer el contenido de un archivo
```
cat archivo.jsx
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

Para ver la historia de nuestros archivos, los commits, el usuario que lo cambió, cuando se realizaron los cambios etc. seguidamente ponemos el nombre de nuestro archivo.
```
git log archivo.jsx
```
