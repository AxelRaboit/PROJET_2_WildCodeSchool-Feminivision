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


