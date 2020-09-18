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
	
