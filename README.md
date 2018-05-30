# Mise en place du projet

Cloner les sources du vagrant utilisées pour ce projet :

`git clone git@github.com:noemieleitao/vagrant.git`

Exécution de vagrant pour obtenir le projet en local :

`vagrant up`

## Vérification de la bonne mise en place du projet
Deux solutions :
- à la suite de la commande précédente, un dossier contenant les sources du projet nommé "drupal" se situe à la racine du projet
- une erreur s'est produite, il faut donc cloner manuellement le projet. Dans ce cas exécutez les commandes suivantes :
```
cd vagrant
git clone git@github.com:noemieleitao/visuel_upjv.git drupal
vagrant up
``` 

## Ajout de la base de données
Remplacer my_project, la base de données créée, par la base de données présente dans vagrant/drupal/database/my_project.sql

Remarque : si vous utilisez phpmyadmin pour remplacer la base de données, l'importation des données peut bloquer à cause de la taille du fichier dépassant 2 Mo. Dans ce cas, compressez en fichier zip puis réessayez.

# Url
url|utilité
---|-------
http://localhost:8090 | accès au site 
http://localhost:8090/admin | accès à l'administration du site
http://localhost:8090/phpmyadmin/ | accès à phpmyadmin

# Identifiant

---|-------
Nom d'utilisateur : | my_user
Mot de passe : | my_password
