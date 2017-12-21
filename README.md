----------------------------------COMANDOS------------------------------------
Una vez instalado git, debes configurarlo:

git config --global user.name  "xxxxxxxxxxxx"
git config --global user.email "xxxxxxxxxxx"

Generando tú public Key:
ssh-keygen

Leer dicha llave para copiarla en GitHub
cat ~/.ssh/id_rsa.pub 

Arrancando el proyecto
git init:							Crea un nuevo repositorio(en el directorio que estamos ubicados)
touch:								Crear un nuevo archivo(README2)			
git add<nombrearchivo> o git add .:	Adiciona el archivo creado(README2)
git commit -m <msg>:
git remote add origin:  			Trae los archivos a local desde la cuenta git(url de git)
git pull origin master: 			Prepara para llevar a cuenta git del ordenador todos los archivos locales
git push origin master:				Envia todos los archivos preparados a la cuenta git
git status:							estado del repositorio configurado


----------------------------------------------------------------------
TAREAS: 

#Clonar un proyecto
1. crear el directorio mkdir <nombredeproyecto>
2. ejecutar el comando git init para instanciar el repositorio
3. ejecutar el comando git remote add <url en git del proyecto>(si no presenta msg esta todo bien)
4. ejecutar el comando git pull origin master (se empieza a descargar el proyecto y listo a trabajar)

#Crear un archivo
1.touch <nombrearchivo>
2.git add<nombrearchivo> o git add .
3.git commit -m <"Descripcion del cambio entre comillas">

#Creacion de Ramas
1. git branch <nombredelarama>

#Moverte a una rama a otra
1.git checkout <nombredelarama>

#Agregar una rama al archivo master o principal
1.git merge <nombredelarama>


#BORRAR BRANCH
$ git branch -d <nombredelarama>
 
#BORRAR BRANCH REMOTO
$ git push origin :the_remote_branch


NOTAS:

1)Fork: me crea una nueva versión del proyecto al que quiero colaborar dentro de github