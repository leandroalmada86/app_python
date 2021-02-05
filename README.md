# app_python

Écrire une image Docker avec les spécifications suivantes :

๏ une image alpine de base (se renseigner sur les images alpines, quels sont leur
avantage par rapport à une image normale?)

๏ python3.x, pip3 et vim

๏ une installation automatique du fichier requirements.txt (qui contiendra entre autre la
librairie virtualenv) que vous écrirez à la racine de votre application. Renseignez vous
sur ce fichier requirements.txt, que fait il, pourquoi est il utile?

๏ un répertoire app (dans lequel se trouvera l’application app.py)

๏ une exposition du port de l’application

๏ pour finir builder un container qui lancera l’application lors de sa création

๏ (BONUS) se renseigner sur le micro-framework web Flask et personnaliser
l’application


Docker:

docker build <pathFolder> -t <imageName> : Build le conteneur
docker run <imageName> : Execute l'image 
docker ps -a : Listes des conteneurs connu
docker start <containerName> : Démarre le containeur
docker stop <containerName> : Arrete le containeur
docker rm <containerName> : Supprime le containeur
docker rmi <imageName> : Supprime l'image 


Pour set le port:

sudo docker run -p 8080:5000 pythonimage:latest

docker inspect <containerName>