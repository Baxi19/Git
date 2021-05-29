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

Borrar un archivo que hayamos añadido, para eliminarlo por completo de nuestra RAM usamos **git rm --cached** o bien puedes remover un solo archivo adjuntando el nombre del mismo y su extencion

```
git rm archivo.jsx

# se usa para devolver el archivo que se tiene en ram cuando escribimos 
# git add lo devuleve a estado natural mientra esta en staging
git rm --cached
```

Añadir un commit a nuestra rama, también podemos ponerle un **-m** seguidamente ponemos entre comillas un mensaje que represente el commit. 

Importante en caso de que solo coloque **git commit** el sistema le abrira **VIM** un editor de codigo basado en linea de comandos,   solicita que ingrese un msj, para insertar texto se hace con la letra **Scape** + **i** luego se puede insertar texto,al hacerlo y para poder salir del editor es necesario usar la combinacion de teclas *Esc* + *Shift* + *z* + *z* y de esa manera se ejecuta el commit correctamente
```
git commit -m "Mensaje que represente el commit"
```

Para ver la historia de nuestros archivos, los commits, el usuario que lo cambió, cuando se realizaron los cambios etc. seguidamente ponemos el nombre de nuestro archivo.
```
git log archivo.jsx
```

Mostrar el contenido de un archivo
```
cat archivo.jsx 
```

Para ver los cambios que se le han realizado a un archivo :fire: es super importante en casos de que necesites ver que cambios han sido realizados en un archivo especifico
```
git show archivo.jsx
```

Listado de carpetas en donde me encuentro es decir **dir** en Windows
```
ls 
```

Para saber la ubicacion actual
```
pwd 
```

Crear nueva carpeta
```
mkdir nombreCarpeta
```

Crear archivo vacio
```
touch archivo.extencion
```

Ver cambios entre commits especificos, es muy importante para saber los cambios entre los diferentes commits
```
git diff commitMasAntiguo commitMasReciente
```

Para volver a un commit especifico, se puede observar el nombre del commit al que se quiere ir con el comando **git log** luego que se tiene, se puede borrar todo lo que se creo de un commit especifico en adelante
```
git reset idCommit --hard
```

Al igual que el anterior regresa a un commit especifico, pero deja lo que esta en staging, continua ahi mismo, es decir, si a realizado cambios y le ha dado **git add archivo.jsx**, esos cambios continuan ahi disponibles para el proximo commit (Solo el directorio de trabajo vuelve a la version anterior
```
git reset idCommit --soft
```



historial de comandos utilizados durante esa sesion
```
history 
```

ayuda sobre el comando
```
comando --help
```

traer cambios realizado
```
checkout 
```
