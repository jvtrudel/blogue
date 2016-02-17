

# Nouvelle base de donnée

## Ouverture de mySQL en command-line

    mysql -u root -p

## Création d'une base de donnée

    create database <nom de la base>;

## Création d'un nouvel utilisateur

    create user <nom du user> @ 'localhost' identified by <password>;

## Donner les permissions à un utilisateur

    GRANT <permission> ON <database>.<table> TO 'user'@'localhost';


# Gestion des utilisateurs
[inspection des utilisateurs](http://alvinalexander.com/blog/post/mysql/show-users-i-ve-created-in-mysql-database)

    select * from mysql.user;

# Inspection

## Quelles bases de donneés sont disponibles

    show database;

## Voir si quelles sont les tables qui existent

    show tables;

## Voir le schema d'une table

    describe <nom de la table>;

## Voir le contenu d'une table

    select * from <nom de la table>;

# Création de tables

    create table <nom de la table>;

## selection de la base

    use <base de donnée>

## Destruction d'une ligne

    delete from <table> where <critère>;

## Destruction d'une table

    drop table <table à détruire>;


## importation de fichier csv

   load data local infile '/Users/manitou6/Desktop/BDplusWebDynamique/givenData/support/importations/tableClasse.txt' into table Classe
   fields terminated by ';'
   enclosed by '"'
   lines terminated by '\n'

# accès/opération serveur

## Démmarage du serveur

   <!-- sudo port load mysql56-server !-->

    mysql.serveur start


# Importation et Exportation de base de données

## Exportation mysql

    mysqldump -u<user> -p <nom BD> > <nom fichier>.sql

## Importation de BD entière

    mysql -u username -ppassword databasename < filename.sql

# Librairie PHP PDO

## Ressources

  - [connection à DB (w3school) ](http://www.w3schools.com/php/php_mysql_connect.asp)
  - [insertion data ds db (w3school)](http://www.w3schools.com/php/php_mysql_insert.asp)

  # Commandes

    - CREATE TABLE : créer une nouvelle table.
    - INSERT INTO : ajouter une nouvelle ligne.
    - SELECT : selectionne des données d'une table.
    - UPDATE : modifie les valeurs d'une colonne.
    - ALTER TABLE : modifie la structure d'une table.
    - DELETE FROM : efface une ligne d'une table

# Ressources internet

[Tuto+python](http://zetcode.com/db/mysqlpython/)
