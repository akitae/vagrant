# Mise en place du projet

Cloner les sources du vagrant utilisé pour ce projet :

`git clone git@github.com:noemieleitao/vagrant.git`

Exécution de vagrant pour obtenir le projet en local :

`vagrant up`

## Vérification de la bonne mise en place du projet
Deux solutions :
- à la suite de la commande précédente, un dossier contenant les sources du projet nommé "drupal" se situe à la racine du projet
- une erreur c'est produite est il faut clonné manuellement le projet. Pour ce cas exécutez les commandes suivantes :
```
cd vagrant
git clone git@github.com:noemieleitao/visuel_upjv.git drupal
vagrant up
``` 

## Ajout de la base de donnée
Remplacer la base de donnée crée par la base de donnée présente dans vagrant/drupal/database/my_project.sql

Remarque : si vous utilisez phpmyadmin pour remplacer la base de donnée, il se peut que ce soit refusé du à sa taille. Dans ce cas, compresser avec 
zip puis réessayer.

# Url
url|utilité
---|-------
http://localhost:8090 | accès au site 
http://localhost:8090/admin | accès à l'administration du site
http://localhost:8090/phpmyadmin/ | accès à phpmyadmin
