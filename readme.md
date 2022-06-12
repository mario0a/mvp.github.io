# site d'annonce version 1.0
ngonaAnnonce est un site d'annonce en ligne qui permet au personnes souhaitant postuler une annonce de le faire gratuitement

# pour lancer le projet  il faut:
0) php bin/console doctrine:database:create  pour creer la base de donnee
1) composer install
2) docker-compose up -d  pour lancer la base de donné et mailler si posible
3) npm install 
4) npm run build pour lancer webpack
5) symfony serve -d  : pour lancer le server de l'application

# les Installations necessaires apres avoir créer le projet avec symfony new --full "nom_du_projet"

# creation de la base de donnée avec docker
symfony console make:docker:database
ext:
A) Run docker-compose up -d database to start your database container
or docker-compose up -d to start all of them.

B) If you are using the Symfony Binary, it will detect the new service automatically.
Run symfony var:export --multiline to see the environment variables the binary is exposing.
These will override any values you have in your .env files.

C) Run "docker-compose stop" will stop all the containers in docker-compose.yaml.
docker-compose down will stop and destroy the containers.

# lancement du contenair pour la base de donnee  et de mailler pour les mail
docker-compose up -d
#lancement du server interne de symfony en  faisant
symfony serve -d
# test unitaire sur les enttés creation de la classe
symfony console make:unit-test
#lancement du test de la  class
php bin/phpunit --testdox

# installation de webpack
composer req symfony/webpack-encore-bundlE
# dans le fichier assert on remplace css par scss
# pour builder et lancement de webpack
vider le fichier app.scss
npm run build
# decommender le ligne 59 de webpack.config.js
.enableSassLoader()

#lancer un buil
npm run build

#on install
npm install postcss-loader autoprefixer --dev

# dans la racine du projet, on créé un fichier postcss.config.js
on met :dans le fichier
module.exports={
plugins:{
autprefixer:{}
}
}
#lancer un buil
npm run build

# installation de bootstrap deriere version avec npm
npm install bootstrap
npm install @popperjs/core


# on importe le fichier bootstrap dans asserts/app.js
import { Tooltip,Toast,Popover} from "bootstrap";
on importe aussi dans asserts/app.scss
@import "~bootstrap/scss/bootstrap";

#lancer un buil
npm run build 
#creation du template
symfony console make:controller Acceuil
# demarrage de l'environnement docker pour la base de onnee et mailler
composer install
npm install
npm run build
docker-compose up -d 
# lancement du server 
symfony serve -d
# on met un navbar bootstrap de le templete index 

# ajout de l'authentifiaction
symfony console make:auth

#ajoute de  la page login
symfony console make:auth
# pour ajouter le remember me il faut suivre le lien
https://symfony.com/doc/current/security/remember_me.html






