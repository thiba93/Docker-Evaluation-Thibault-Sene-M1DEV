Petite Application Flask avec Docker Compose
Cette application est une simple page Flask qui dit "Bonjour" et qui est conteneurisée avec Docker.

Prérequis : 
Installez Docker et Docker Compose.
Démarrer l'application Docker sur votre ordinateur 
Clonez ce projet.

Si vous voulez lancer l'application avec les instructions de Dockerfile il vous faudra tapez ces commandes :

dcker build -t flask-app .   ( flask-app etant le nom de votre applicaiton )

puis vous allez devoir le lancer via cette commande : 

docker run -d -p 8080:5000 flask-app

Si vous voulez lancer l'application avec Docker Compose il vous faudra taper cette commande dans le terminal à la racine de ce projet : 

docker-compose up

Grâce à ces deux commandes vous allez pouvoir : 

Ouvrez un navigateur et allez sur http://localhost:5000 pour voir l’appli en action. Vous aurez :

La page d'accueil à l'accueil qui dit bienvenue.
Une page /apropos avec une petite description.


Pour arrêter l'application 

Si vous avez utilisé crée l'image vous-même pour ensuite le lancer il vous faudra :

docker ps

Pour recuperer toutes les informations de tous les conteneur en cours d'éxécution puis

docker stop <id_conteneur>


Si vous avez utilise docker-compose up il vous faudra faire la commande :
docker-compose down



docker-compose down
#   D o c k e r - E v a l u a t i o n - T h i b a u l t - S e n e - M 1 D E V  
 