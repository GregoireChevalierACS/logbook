**Logbook projets**


*06 Août 2021*
- Mise à jour de Docker
- Mise à jour d'Ubuntu 20.04 dans wsl2
- Sudo apt atoremove dans Ubuntu 20.04 pour clean up
- Installation de PHP 7.4 dans Ubuntu 20.04
- Installation de Composer (1.10) dans Ubuntu 20.04
- Installation de la CLI de symfony dans Ubuntu 20.04
- Installation de simplexml (paquet requis pour symfony) dans Ubuntu 20.04
- Installation de Doctrine (2.7.2) dans Ubuntu 20.04
- Installation du module intl de PHP (requis pour les validators) dans Ubuntu 20.04

Requirements met for symfony

- Rename du repo Projet PHP de github en Projet Php Symfony TDD
- Clone du projet Php Symfony TDD dans Ubuntu 20.04
- Cleaning du repo
- Création du squelette symfony avec ```symfony new projet_symfony_tdd --full```


*07 Août 2021*


Suivi des prérequis pour installer PHPUnit (https://phpunit.readthedocs.io/fr/latest/installation.html)


- Installation d'xDebug dans le dossier Hub d'Ubuntu 20.04
- DL et installation de PHPUnit 9.5.8 global dans Ubuntu 20.04
- Création de controleur test dans le projet symfony
- Installation & activation de l'extension mysql pour pdo dans le php.ini du projet symfony
- Erreur symfony : An exception occurred in driver: could not find driver. Semble venir du fait que je suis sous wsl2. A creuser

*08 Août 2021*


- Installation de la CLI symfony sur windows
- Installation de Composer sur windows avec creation du php.ini
- Initialisation d'un projet symfony avec la commande composer, la cli de symfony ne marchant apparemment pas.
- Création du fichier .php-version avec 7.4.9 dedans pour harmoniser avec la version de wamp et résoudre le problème de no input file specified

- Résolution du problème  An exception occurred in driver: could not find driver sous WSL2 en changeant dans le .env la db de postgre (defaut) à mysql (lignes 30&31)
- Arrivée sur An exception occurred in driver: SQLSTATE[HY000] [2002] Connection refused
- Dive dans le DBAL (database abstraction layer (DBAL) https://www.doctrine-project.org/projects/doctrine-dbal/en/latest/index.html)
- Installation et déploiement de mysql dans WSL2 pour pallier à hy0000 2002 (https://dev.mysql.com/doc/refman/8.0/en/linux-installation.html)
- Installation de mysql dans ubuntu wslé (https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04-fr)
- Workaround suite à l'erreur 'cant connect to local mysql server through socket' (https://medium.com/@alef.duarte/cant-connect-to-local-mysql-server-through-socket-var-run-mysqld-mysqld-sock-155d580f3a06)
- MySql voué à échouer, installer mariadb sur ubuntu (https://www.digitalocean.com/community/tutorials/how-to-install-mariadb-on-ubuntu-20-04-quickstart-fr)


*09 Août 2021*


- Setup de clé ssh sur pc fixe perso
- Résolution du problème (WslRegisterDistribution failed with error: 0x8007019e) pour utilisation d'ubuntu sur pcfixe
- Setup de clé ssh sur ubuntu 20.04 pc fixe perso
- Install vscode sur ubuntu 20.04 pc fixe perso


*10 Août 2021*

- Update de git à la version 2.32.0.2 sur pc fixe perso
- Clone du projet Symfony TDD sur ubuntu 20.04 pc fixe perso
- Installation de php 7.4 sur ubuntu 20.04 pc fixe perso
- Installation de Composer sur ubuntu 20.04 pc fixe perso
- Installation de la cli de symfony sur ubuntu 20.04 pc fixe perso
- Installation des dépendances nécessaires à symfony sur ubuntu 20.04 pc fixe perso
- Installation de apt-get install php-mysql sur ubuntu 20.04 pc fixe perso, qui semble causer le probleme An exception occurred in driver: SQLSTATE[HY000] [2002] Connection refused

- Tenter de remonter le projet avec un docker de services qui marchent


*11 Août 2021*

- Clone du projet symfony tdd dans dossier www wamp pc perso
- Composer install
- Modification du .env ligne 30 :
```DATABASE_URL="mysql://root:@127.0.0.1:3306/db_name?serverVersion=5.7"```
remplacement de db_user:db_password
- php bin/console doctrine:database:create pour créer la bdd qui prend  le nom renseigné dans le .env (db_name)

*16 Août 2021*

- Reprise du projet paris sportif
- Composer install des dépendances
- Migrations bdd et fixtures de base

- Projet test laravel
- Activation de la distri ubuntu 20.04 dans les parametres/Resources/Wsl integration
- Dans ubuntu, commande ```curl -s https://laravel.build/example-app | bash``` pour créer un projet template laravel
- Dans le dossier test, commande : ```./vendor/bin/sail up``` pour créer, instaler et monter une image  de la CLI Laravel via docker


*17 Août*

- Projet test laravel fonctionnel gité
- Création de route perso


*18 Août*

- Récupération dossier node stage


*26 Août*

- Définition du planning pour les 7 jours à venir


*27 Août*

- Reprise du projet tdt en tdd
- Clean up du repo et revue des objectifs
- Installation de phpunit et premier test requete
- Création de l'index php
- Abandon test requete et premiers tests fonctionnels


*28 Août*

- Lecture de doc (https://phpunit.readthedocs.io/fr/latest/extending-phpunit.html)
- Pour tester le contenu des champs, il faudra utiliser symfony