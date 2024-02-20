# Ejercicio 1  
## 1.1 Crear directorio llamado Repo Test:  
Abrimos git bash y hacemos comando 'pwd' para ver dónde nos posicionamos. Después vemos el contenido del directorio utilizando el comando 'ls' y nos dirigimos a la carpeta donde queremos trabajar usando 'cd Documents/', 'cd Bootcamp Java1/ (tab para autocompletar).  

Una vez en la carpeta donde queremos trabajar creamos una carpeta para nuestro repositorio, 'mkdir "Repo test". Para ver que se ha creado correctamente usamos 'ls'.  

Para poder trabajar con un repositorio local y remoto tenemos que configurar user.name y user.email:  
- git config, git config user.name "Thirza Visser"
- git config, git config user.email "thirzavisser95@gmail.com"  

Entramos en la carpeta Repo test, cd Repo test/, y hacemos un git init para inicializar el repositorio local.

Podemos identificar que el repositorio se ha inicializado correctamente visualizando las carpetas ocultas y que haya allí un .git.  

Si se hace un git log, se puede ver que todavía no hay commits y con el git status vemos que no hay nada para hacer commit.

## 1.2 Añadir documento readme.md  

He abierto Visual Studio Code utilizando 'code .' y he añadido un documento readme donde estoy documentando ahora todos los cambios que hacemos.  

## 1.3 Añadir el readme.me al staging area  

Podemos añadir el documento readme.md al staging area utilizando el comando 'git add readme.md'.  

Luego hacemos un git status y vemos lo siguiente:  
\*Añadir foto  

Hacemos el comando 'git commit -m "añadir documento readme".  
\*Añadir foto  

El fichero se encuentra ahora en la caja de committed del File status Lifecycle.