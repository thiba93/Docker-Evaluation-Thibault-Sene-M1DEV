Petite Application Flask avec Docker Compose
Cette application est une simple page Flask qui dit "Bonjour" et qui est conteneurisée avec Docker.

Prérequis :
Installez Docker et Docker Compose.
Démarrez l'application Docker sur votre ordinateur.
Clonez ce projet.
Si vous voulez lancer l'application avec les instructions de Dockerfile, il vous faudra taper ces commandes :

docker build -t flask-app .   (flask-app étant le nom de votre application)
Puis vous allez devoir le lancer via cette commande :

docker run -d -p 5000:5000 flask-app
Si vous voulez lancer l'application avec Docker Compose, il vous faudra taper cette commande dans le terminal à la racine de ce projet :


docker-compose up
Grâce à ces deux commandes, vous allez pouvoir :

Ouvrir un navigateur et aller sur http://localhost:5000 pour voir l’appli en action.
Vous aurez :

La page d'accueil à l'accueil qui dit bienvenue.
Une page /apropos avec une petite description.
Pour arrêter l'application
Si vous avez utilisé l'image créée vous-même pour ensuite la lancer, il vous faudra :

docker ps
Pour récupérer toutes les informations de tous les conteneurs en cours d'exécution, puis :

docker stop <id_conteneur>
Si vous avez utilisé docker-compose up, il vous faudra faire la commande :

docker-compose down
