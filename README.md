# Mise en place du projet

Clonez les sources du vagrant utilisées pour ce projet :

`git clone https://github.com/noemieleitao/vagrant.git`

Ensuite chargez les sources du projet drupal :
```
cd vagrant
git clone https://github.com/noemieleitao/visuel_upjv.git drupal
```

Puis exécutez la commande suivante :
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

Pour remédier à cela connectez-vous à l'accès phpmyadmin avec les identifiants :  
Nom d'utilisateur : root   
Mot de passe : root  

Supprimez la base de données my_project.

Importez la base de données située à l'emplacement `vagrant/drupal/database/my_project.sql`.

Note : Compressez au préalable la base dans un format .zip.
