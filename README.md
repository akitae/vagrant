# Mise en place du projet

Cloner les sources du vagrant utilisé pour ce projet :

`git clone git@github.com:noemieleitao/vagrant.git`

Ensuite charger les sources du projet drupal :
```
cd vagrant
git clone git@github.com:noemieleitao/visuel_upjv.git drupal
```

Puis exécuter la commande suivante :
`vagrant up`

# Url
Url|Utilité
---|-------
http://localhost:8090 | accès au site 
http://localhost:8090/admin | accès à l'administration du site
http://localhost:8090/phpmyadmin/ | accès à phpmyadmin

# Identifiant
Donnée|Valeur
---|-------
Nom d'utilisateur | my_user
Mot de passe : | my_password

# Vérification de la bonne mise en place du projet

Dans le cas où vous arrivez sur la page d'installation en accédant au site, cela signifie que la base de données ne s'est pas correctement installée.

Pour remédier à cela connectez-vous à l'accès phpmyadmin avec les identifiants root/root.
Supprimer la base de données my_project.
Importer la base de données situé à l'emplacement `vagrant/drupal/database/my_project.sql`.
Note : Compresser au préalable la base dans un format .zip.


