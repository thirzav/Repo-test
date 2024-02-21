# Ejercicio 1  
## 1.1 Crear directorio llamado Repo Test:  
Abrimos **git bash** y hacemos comando **pwd** para ver dónde nos posicionamos. Después vemos el contenido del directorio utilizando el comando **ls**:   
  
![alt text](<imagenes repo test 1/Image 1.png>)
  
Nos dirigimos a la carpeta donde queremos trabajar usando en este caso: **cd OneDrive**, **cd Documentos/**, **cd Bootcamp Java1/** *(tab para autocompletar)*:  

![alt text](<imagenes repo test 1/Image 2.png>)  

Una vez en la carpeta donde queremos trabajar creamos una carpeta para nuestro repositorio con el siguiente comando: **mkdir "Repo test**. Para ver que se ha creado correctamente usamos el comando **ls**, lo cual se puede ver en la imagen arriba.  
  
Para poder trabajar con un repositorio local y remoto tenemos que configurar user.name y user.email utilizando los siguientes comandos:  
- **git config, git config user.name "Thirza Visser"**   
  ![alt text](<imagenes repo test 1/Image 3.png>)

- **git config, git config user.email "thirzavisser95@gmail.com"** 
  ![alt text](<imagenes repo test 1/Image 4.png>)
  
Entramos en la carpeta Repo test, *cd Repo test/*, y hacemos un comando **git init** para inicializar el repositorio local.
  
![alt text](<imagenes repo test 1/Image 5.png>)

Podemos identificar que el repositorio se ha inicializado correctamente visualizando las carpetas ocultas y que haya allí un ***.git***.  
  
![alt text](<imagenes repo test 1/Image 6.png>)

Si ejecutamos el comando **git log**, podemos ver que todavía no hay commits y con **el git status** vemos que no hay nada para hacer commit.

## 1.2 Añadir documento readme.md  

Abrimos Visual Studio Code utilizando el comando **code .** y añadimos un documento readme donde estoy documentando ahora todos los cambios que hacemos.  
  
![alt text](<imagenes repo test 1/Image 7.png>)

## 1.3 Añadir el readme.me al staging area  

Podemos añadir el documento readme.md al *staging area* utilizando el comando **git add readme.md**.  

Luego hacemos un **git status** y vemos lo siguiente (ver imagen abajo), hacemos el comando **git commit -m "añadir documento readme"**.  

![alt text](<imagenes repo test 1/Image 8.png>)

El fichero se encuentra ahora en la caja de *committed del File status Lifecycle*.  
  
Podemos comprobar que el fichero está en el *staging area* empleando el comando **git status**:  
  
![alt text](<imagenes repo test 1/Image 8a.png>)
  
## 1.4 Subir ficheros al repositorio remoto  

Para subir un fichero al repositorio remoto utilizamos el comando **git push**. En este caso no podemos subir el fichero al repositorio remoto todavía, porque no está asociado a ninguno *(pongo un ejemplo de RepoEx01, el proceso es el mismo, sólo cambian los nombres que hemos puesto, ya que en Repo test ya lo tenía asociado)*:  
  
![alt text](<imagenes repo test 1/Image 9b.png>) 
  
En la imagen podemos ver que al hacer el **git push** nos dice: ***fatal***. Nos responde así, porque no tiene un repositorio remoto asociado así que no ha podido completar este comando.  

## 1.5 Git remote -v  

Como no hay un repositorio asociado no aparece nada al hacer el comando **git remote -v** *(que normalmente muestra con que repositorio remoto está asociado el repositorio local)*.  
  
![alt text](<imagenes repo test 1/Image 10.png>)

## 1.6 Crear repositorio remoto  

En la página de **Github** creamos un repositorio remoto. Damos al **+**, **new repository**:   
  
![alt text](<imagenes repo test 1/Image 11.png>)  
  
Damos un nombre al repositorio y lo creamos. Vamos a **code** y copiamos las líneas:

![alt text](<imagenes repo test 1/Image 12.png>)  

Añadimos las líneas en la terminal de Visual Studio Code para asociar el repositorio remoto al repositorio local.  
  
![alt text](<imagenes repo test 1/Image 13.png>)

## 1.7 Git remote -v  

Ahora que hemos creado y asociado el repositorio remoto, al hacer el comando **git remote -v** aparece: 

![alt text](<imagenes repo test 1/Image 14.png>)

## 1.8 Subir cambios al repositorio remoto  

Para subir los cambios hacemos un **git add .** para incluir todos los documentos. Luego un **git commit -m "añadir documento readme"**. Y para subirlo un **git push -u origin main**.  
  
![alt text](<imagenes repo test 1/Image 15.png>)

## 1.9 Comprobar repositorio remoto  

Para comprobar que el fichero ha subido correctamente vemos el commit en el repositorio remoto *(ahora ya aparecen más commits en la imagen, los cuales he ido haciendo mientras escribía este documento)*.  
  
![alt text](<imagenes repo test 1/Image 16.png>)