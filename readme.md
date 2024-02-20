# Ejercicio 1  
## 1.1 Crear directorio llamado Repo Test:  
Abrimos git bash y hacemos comando 'pwd' para ver dónde nos posicionamos. Después vemos el contenido del directorio utilizando el comando 'ls' y nos dirigimos a la carpeta donde queremos trabajar usando 'cd Documents/', 'cd Bootcamp Java1/ (tab para autocompletar).  
  
**\* añadir image 1 y image 2**

Una vez en la carpeta donde queremos trabajar creamos una carpeta para nuestro repositorio, 'mkdir "Repo test". Para ver que se ha creado correctamente usamos 'ls', lo cual se puede ver en la imagen arriba.  

Para poder trabajar con un repositorio local y remoto tenemos que configurar user.name y user.email:  
- git config, git config user.name "Thirza Visser" **\*añadir image 3**
- git config, git config user.email "thirzavisser95@gmail.com" **\* añadir image 4**  

Entramos en la carpeta Repo test, cd Repo test/, y hacemos un git init para inicializar el repositorio local.
  
**\*añadir image 5**

Podemos identificar que el repositorio se ha inicializado correctamente visualizando las carpetas ocultas y que haya allí un .git.  
  
**\*añadir image 6**

Si se hace un git log, se puede ver que todavía no hay commits y con el git status vemos que no hay nada para hacer commit.

## 1.2 Añadir documento readme.md  

He abierto Visual Studio Code utilizando 'code .' y he añadido un documento readme donde estoy documentando ahora todos los cambios que hacemos.  
  
**\*añadir image 7**

## 1.3 Añadir el readme.me al staging area  

Podemos añadir el documento readme.md al staging area utilizando el comando 'git add readme.md'.  

Luego hacemos un git status y vemos lo siguiente (ver imagen posterior), hacemos el comando 'git commit -m "añadir documento readme".  
**\*Añadir image 8**  

El fichero se encuentra ahora en la caja de committed del File status Lifecycle.  

## 1.4 Subir ficheros al repositorio remoto  

No se puede subir todavía, porque no está asociado a un repositorio remoto (pongo ejemplo de RepoEx01):  
  
**\*añadir image 9**

## 1.5 Git remote -v  

Como no hay un repositorio asociado no aparece nada.  
  
**\*añadir image 10**

## 1.6 Crear repositorio remoto  

En la página de Github creamos un repositorio remoto. Damos al '+', 'new repository', le damos un nombre y lo creamos. Vamos a 'code' y copiamos las líneas.  
  
**\*añadir image 11 y 12**  

Añadimos las líneas en la terminal de Visual Studio Code para asociar el repositorio remoto al repositorio local.  
  
**\*añadir image 13**

## 1.7 Git remote -v  

Ahora que hemos creado y asociado el repositorio remoto, al hacer el comando 'git remote -v' aparece . 

**\*añadir image 14** 

## 1.8 Subir cambios al repositorio remoto  

Para subir los cambios hacemos un 'git add .' para incluir todos los documentos. Luego un git commit -m "añadir documento readme". Y para subirlo un 'git push -u origin main'.  
  
**\*añadir image 15  

## 1.9 Comprobar repositorio remoto  

Vemos el commit en el repositorio remoto (ahora ya aparecen más commits en el documento, los cuales he ido haciendo mientras escribía este documento).  
  
**\*añadir image 16**