Comment vérifier la configuration actuelle de Git sur votre machine, notamment le nom d’utilisateur et l’adresse e-mail ?

Soit :

bash

git config --global user.name
git config --global user.email

Soit :

bash

git config --list

Cela affiche toutes les configurations.

Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installation de Git ?

bash

git config --global user.email "nouvelle.adresse@example.com"

Si vous avez oublié de créer un fichier README.md lors de l'initialisation du projet, comment pouvez-vous l'ajouter après coup et commiter les changements ?

bash

touch README.md
git add README.md
git commit -m "Ajout du fichier README.md"




Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la création du projet ?
Utilisez la commande :

bash

git remote add origin <URL_DU_DEPOT>

Comment annuler les modifications locales d'un fichier avant de les ajouter à l'index ?
Utilisez :

bash

git checkout -- nom_du_fichier

Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?
Exécutez :

bash

git status

Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?
Utilisez :

bash

git fetch origin

Comment supprimer une branche locale après l'avoir fusionnée dans master ?
Exécutez :

bash

git branch -d nom_de_la_branche

Comment interrompre un rebase en cours si vous avez commis une erreur ?
Utilisez :

bash

git rebase --abort

Comment lister les commits qui vont être rebasés avant de lancer un rebase ?
Exécutez :

bash

git log --oneline ma-fonctionnalite ^master

Comment afficher la liste des branches actives et en cours de développement dans Git Flow ?
Utilisez :

bash

git flow feature list

Comment annuler une branche de correctif (hotfix) avant de la finaliser si vous constatez une erreur ?
Exécutez :

bash

git flow hotfix cancel nom_du_correctif
