# Campusciffrafa

# 2.1 REPOSITORIO CAMPUSCIFF (I)
## 1 Crear un repositorio en vuestro GitHub llamado campusciff.

# 2.2 REPOSITORIO CAMPUSCIFF (II)
## 1 Clonar vuestro repositio en local.
	git clone https://github.com/solkido/Campusciffrafa.git

# 2.3 README
## 1 Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md.
	Este se ha creado automaticamente al crear mi repositorio al seleccionar la opcion de que se creara
	
# 2.4 COMMIT INICIAL
## 1 Añadir al README.md los comanddos utilizados hasta ahora y hacer un coomit inicial con el 	
	git add . --all
	git commit -m "Commit inicial"

# 2.5 PUSH INICIAL
## 1 Subir los cambios al repositorio remoto.
	git push
	
# 2.6 IGNORAR ARCHIVOS (I)
## 1 Crear en el repositorio local un fichero llamado privado.txt.
	touch privado.txt
    
## 2 Crear en el repositorio local una carpeta llamada privada.
 	mkdir privada
	
 # 2.7 IGNORAR ARCHIVOS (II)
## 1 Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.
	echo "privado.txt" > .gitignore
	echo "/privada" > .gitignore
	git add .
    git commit -m "añadido fichero .gitignore"
	
# 2.8 AÑADIR FICHERO 1.TXT
## 1 Añadir fichero 1.txt al repositorio local.
	touch 1.txt
	git add . -all
	git commit -m "añadido 1.txt"
	
# 2.9 CREAR EL TAG V0.1
## 1 Crear un tag v0.1.
	git tag v0.1
	
# 2.10 SUBIR EL TAG V0.1
## 1 Subir los cambios al repositorio remoto.
 	git push --tag

# 2.11 CUENTA DE GITHUB
## 1 Poner una foto en vuestro perfil de GitHub
 ![github](https://user-images.githubusercontent.com/39245090/93825762-34beba80-fc66-11ea-8363-253486657fdb.png)

# 2.13 CREAR UNA TABLA
## 1 Crear una tabla de este estilo en el fichero README.md con la información de varios de tus 
compañeros de clase:

| NOMBRE | GITHUB |
| -- | -- |
| David | https://github.com/dvidgb/campusciff |
| Alejandro | https://github.com/aguerra952/campusciff |

# Avanzado


# 2.2 CREAR UNA RAMA V0.2
## 1 Crear una rama v0.2.
	git branch v0.2
## 2 Posiciona tu carpeta de trabajo en esta rama.
	git checkout v0.2

# 2.3 AÑADIR FICHERO 2.TXT
## 1 Añadir un fichero 2.txt en la rama v0.2.
	touch 2.txt
	git add .
	git commit -m "añadido 2.txt"
    
 # 2.4 CREAR RAMA REMOTA V0.2
## 1 Subir los cambios al reposiorio remoto.
	git push origin v0.2
    
  # 2.5 MERGE DIRECTO
  ## 1 Posicionarse en la rama master.
  	git checkout master
    
## 2 Hacer un merge de la rama v0.2 en la rama master.
	git merge v0.2 -m "merge v0.2 sin conflictos"
 # 2.6 MERGE CON CONFLICTO (I)
## 1 En la rama master poner Hola en el fichero 1.txt y hacer commit.
	git checkout master
	echo "Hola" >> 1.txt
	git add .
	git commit -m "hola en 1.txt"


# 2.7 MERGE CON CONFLICTO (II)
## 1 Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit.
	git checkout v0.2
	echo "Adios" >> 1.txt
	git add .
	git commit -m "adios en 1.txt"

# 2.8 MERGE CON CONFLICTO (III)
## 1 Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2
	git checkout master
	git merge v0.2
	nano 1.txt
	git add .
	git commit -m "arreglado merge en 1.txt"
    
# 2.9 LISTADO DE RAMAS
## 1 Listar las ramas con merge y las ramas sin merge.
	git branch --merged
	git branch --no-merged

# 2.10 ARREGLAR CONFLICTO
 ## 1 Arreglar el conflicto anterior y hacer un commit.
	nano 1.txt
	git add .
	git commit -m "arreglado merge en 1.txt"

# 2.11 BORRAR RAMA
## 1 Crear un tag v0.2
	git tag v0.2
    
## 2 Borrar la rama v0.2
	git branch -d v0.2
    
# 2.12 LISTADO DE CAMBIOS
 ## 1 Listar los distintos commits con sus ramas y sus tags.
	git config --global alias.list 'log --oneline --decorate --graph --all'
	git list

