## Description
Project made in the Wild Code School, a project in partnership with "la pellicule ensorcelée" who highlighting women film directors.

## Try it

1. Clone the repo from Github.
2. Run `composer install`.
3. Create *config/db.php* from *config/db.php.dist* file and add the DB parameters (the database is named 'feminivision') . Don't delete the *.dist* file, it must be kept.
```php
define('APP_DB_HOST', 'your_db_host');
define('APP_DB_NAME', 'feminivision');
define('APP_DB_USER', 'your_db_user_wich_is_not_root');
define('APP_DB_PWD', 'your_db_password');
```
4. Import `feminivision.sql` in your SQL server,
5. Run the internal PHP webserver with `php -S localhost:8000 -t public/`. The option `-t` with `public` as parameter means your localhost will target the `/public` folder.
6. Go to `localhost:8000` with your favorite browser.




## Étapes du projet

## PROJET 2: FEMINIVISION

Le projet est une collaboration avec la pellicule ensorcelée, ce projet consiste à faire un site de recommandation de film crée par des femmes ou par des femmes contributrices de projet cinématographique, avec la possibilité d'ajouter des films, et de faire des recherches avec une selection par filtre.
Il sera réalisé avec PHP / SQL /  POO / TWIG / Base de donnée / Bootstrap.
Nous étions une équipe de 4 personnes, Charlie, Axel, Steve, Axel.

## 20 Octobre 2020
Presentation de chaque projets, avec notre partenaire "La pellicule ensorcelée", 6 projets qui ont été répartis  en 6 groupes.
Nous avons pour notre groupe donc pris "Haut les femmes", un projet qui met en avant les femmes réalisatrices de film cinématographique.

## 21 Octobre 2020
Démarrage du projet.
Nous avons crée un backlog, 
- Quelles seront les fonctionnalités à créer ?
- Dans quel ordre devront-elles être livrées ?
- A qui sont-elles destinées ?
- Qui sera le Product Owner & Scrum Manager
Nous avons par la suite établi la vision du projet,
dans notre cas, offrir un outil de recommandation de film réalisé par des femmes

Définir les priorités des "user stories", qui plus elles sont importantes plus elles se doivent d'être précises.

En parallèle nous avons commencé à crée le wireframe; la version "Desktop" ainsi que la version "Mobile".

(Vue du Trello avancé dans le temp)

<img width="1773" alt="trello-during-project" src="https://user-images.githubusercontent.com/66420167/100485810-cf71c480-3101-11eb-9ea8-0721b1a87956.png">

-----------
## MAQUETTE
-----------

## DESKTOP VERSION:

### HEADER:
![Header](https://user-images.githubusercontent.com/66420167/100485904-2081b880-3102-11eb-915b-f58cc596b914.png)

### FOOTER:
![Footer](https://user-images.githubusercontent.com/66420167/100485965-5f177300-3102-11eb-9efc-b7c1f28fa8ca.png)

### DEROULEMENT DES MENUS:
![Header%20section](https://user-images.githubusercontent.com/66420167/100485993-7f473200-3102-11eb-8d34-2755418c4552.png)

(Nous pouvons y voir que certain menu sont déroulant, et d'autre comme "Année" son sous forme de selection par "range".

### LORS DU CLIC SUR UNE AFFICHE DE FILM:
![Affichage%20film](https://user-images.githubusercontent.com/66420167/100486015-9a19a680-3102-11eb-913f-23664c43dee9.png)

Quand nous cliquons sur une affiche de film, nous pouvons y voir le descriptif de ce dernier;
Le titre, le genre, la date de sortie, la durée du film, le synopsis, le casting, et les hashtag, mais aussi un descriptif de la personne qui à réalisé le film.

Comme nous pouvons le voir ci dessous:
![Option%202%20Affichage%20film%20%E2%80%93%201](https://user-images.githubusercontent.com/66420167/100486039-b0276700-3102-11eb-9935-fbcc3b433db9.png)

Dans le Header se trouve un bouton qui permet d'ajouter un film sur le site, il est représenté par un bouton jaune, lors que l'on clique dessus voilà ce qui apparait:
![Header%20ajouter%20film](https://user-images.githubusercontent.com/66420167/100486056-c2a1a080-3102-11eb-8c40-fb2789aeccf1.png)

Un champ de recherche par titre de film, permettant de chercher un film, la recherche se base sur une recherche du site "imdb" et ainsi pouvoir le proposer à l'aide d'un bouton prévu à cette effet.
Le bouton "Je propose".
![Footer%20ajouter%20film](https://user-images.githubusercontent.com/66420167/100486098-dfd66f00-3102-11eb-9a2e-c7c00a86c434.png)

A chaque instant de la navigation il est possible de faire un retour sur la page d'accueil.

## MOBILE VERSION:

### HEADER:
![Mobile](https://user-images.githubusercontent.com/66420167/100486136-01cff180-3103-11eb-9c5a-1826ba24f7bd.png)

Nous avons voulu faire une version mobile relativement simple, avec un menu hamburger, qui déroule toute la navbar, ainsi qu'une barre de recherche afin de chercher le film que l'on voudrait.

Lors du clic sur le menu hamburger, voici ce que nous proposons, la navbar de la version desktop est de retour,  laissant apparaitre des sections de recherche, 
- "Casting", réalisatrice, réalisateur, atrice, acteur, ...
- "Genre", trié par genre; Action, Aventure, Horreur, Drama, ...
- "Année" une selection par range d'années; de l'année 2xxx à 2xxx .
- "Pays" une selection basé sur le pays d'origine de production.
- "Ajouter un film" qui comme son nom l'indique permet d'ajouter un film qui ne se trouverait pas dans la base de donnée du site.


![Mobile%20%E2%80%93%202](https://user-images.githubusercontent.com/66420167/100486149-14e2c180-3103-11eb-8294-27ddce031434.png)

### AJOUTER UN FILM:

lors du clic sur le bouton "ajouter un film", nous arrivons sur cette page, qui découle de la version desktop, le principe est le meme;
Nous pouvons chercher un film, qui se base sur le site "imdb" pour y ressortir les informations du film rechercher, puis pouvoir le proposer à notre site afin d'y agrandir la base de donnée.

![Mobile%20ajouter%20film](https://user-images.githubusercontent.com/66420167/100486166-2af08200-3103-11eb-8317-1bd5f274011f.png)

---------------
## MAQUETTE FIN
---------------

## 23 Octobre 2020
Ce jour, nous avons travaillé au matin sur le projet, mais tout particulièrement sur la présentation du projet, qui s'est dérouler dans l'après midi.
Nous y avons présenté le projet, la maquette, mais aussi les objectifs, les bonnes pratiques ainsi que les mauvaises,  qui sera Scrum Manager et qui est Product Owner.

## 27 Octobre 2020
Nous avons commencer à travailler sur la création de la base de donnée (MCD / MLD)

## 29 Octobre 2020
Mise en place de la base de donnée avec sa premiere table (Movies), 
Nous avons liéle projet la base de donnée, puis fait le code afin que un film puisse s'afficher sur le site à l'aide d'une requète sql.

<img width="570" alt="bdd_mcd_mld" src="https://user-images.githubusercontent.com/66420167/100486265-7acf4900-3103-11eb-8506-817da0ac647f.png">

## 30 Octobre 2020
Présentation de l'avancer du projet.
Semaine relativement difficile, plonger dans un projet déjà crée, nous devions prendre nos repère pour comprendre l'architecture MVC du projet.
Beaucoup de remise en question et de doute cette semaine là.

## 04 Novembre 2020
Nous avons passé la matiné a résoudre beaucoup de conflit par rapport au pull request, car nous avions mis plusieurs fonctionnalité dans une seul et meme pull request...
Il a donc fallu tout séparer afin de pouvoir faire des pull requests clean.
L'après midi nous avons travaillé sur les chemins de fichier pour que tout celà concorde, nous avons aussi fait un peu de css.

## 05 Novembre 2020
Nous avons travaillé sur le css,  ajouté du contenu dans la base de donnée ( ajouter les 5 premiers films).
Une fonctionnalité qui quand on clique sur un film, elle redirige sur une autre page, grâce à la requete par l'id, et nous avons mis en place le premier contenu de cette derniere page, la prochaine étape sera de la mettre en forme.

## 10 Novembre 2020
- Ajout du formulaire qui permettra à l'utilisateur d'ajouter un film de son choix, en pertinence avec le theme du site.
- -> Fonctionnalité d'upload de l'affiche du film et du contenu, l'affiche sera stocké dans le projet, tandis que le contenu restant dans la base de donnée.
- Ajout d'une table People dans la base de donnée, pour y accueillir les réalisatrice et potentiellement les acteurs de chaque film.
- Recupération de ces données pour les afficher dans la page qui détail le film.
- Création du moteur de recherche de film.

![MCDvendredi132020](https://user-images.githubusercontent.com/66420167/100486322-a9e5ba80-3103-11eb-81b4-db37f9ca4eb6.png)

## 18 Novembre 2020
Nous avons changé plusieurs chose à la demande du client, à savoir la couleur  principal du site, passant du jaune qui faisait trop allo ciné, au bleu.
Nous avons par la suite changé les genres dans le menu déroulant "genres" afin d'y mettre des grandes categories, à savoir,  Fiction, Documentaire, Animation, Expérimental.
Nous avons fait en sorte que tout match (homepage et formulaire) les genres etc...
Le titre du site à été changer pour que ce soit un titre en Français.
(Nous aurions pu garder le titre précédent qui était "Women Directors" si nous avions eu plus de temp pour rendre le site de façon à qu'il soit international et donc dans plusieurs langue, mais étant donné le temp qui nous ai donné nous avons préféré le ciblé en Français, donc avec un titre en français qui est donc devenu "FeminiVision").
Nous avons recrée une toute nouvelle base de donnée, un peu plus fourni, avec de nouvelles tables.
La table "people" à été renommé en "directors", une table "genres a fait son apparition pour y accueillir tout les genres, ainsi que les tables de jointure où les clés étrangères y sont stockées, à savoir "Movies - Directors" qui fait référence à la table "movies" et "Directors" puis  "Movies - Genres" qui fait référence quant à lui à la table "movies" et "genres.

![mld](https://user-images.githubusercontent.com/66420167/100486358-d8fc2c00-3103-11eb-812c-d1aa8816b26b.png)

Nous avons aussi fait en sorte que lors de la recherche de film, quand nous avons plusieurs recherche nous avons chaque films représenté par uniquement l'affiche, par contre si nous avons un unique match alors nous avons directement le détail de l'affiche.

## 24 Novembre 2020
Nous avons fait du css dans la globalité du site, ajouté le footer avec les liens du partenaire et de la wild code school, puis nos lien linkedin de chacun des developpeurs.
Nous avons travaillé sur la fin des fonctionnalités concernant la recherche de film par genre, origine et année, puis aussi la recherche general par titre de film.

## 25 Novembre 2020
Finalisation de la fonctionnalité de rcherche par genre, origine, année, general.
Création de la fonctionnalité qui permet d'indiquer à l'utilisateur que si la recherche ne donne sur rien, le contenu n'a rien à afficher.
Alimentation de la base de donnée, nous avons ajouté une 30ene de films.

## 26 Novembre 2020
Nous avons continué à alimenter la base de donnée pour avoir 31 films au total pour commencer.
Fix des bugs rencontré jusqu'ici.
Ajout de css là où celà est encore manquant et correction des bugs de css.
Finalisation de la fonctionalité "Not Found"
Nettoyage du code, afin de rendre le projet propre.
Le logo favicon a été changé par celui de notre site.

## 27 Novembre 2020
Presentation final du projet, avec le client.
