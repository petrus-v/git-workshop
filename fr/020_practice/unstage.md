# "Unstage" un fichier

Cela arrive d'ajouter un fichier dans l'index, puis, après coup de se dire que
l'on voudrait plutôt faire 2 commits pour avoir un historique plus clair.

Nous cherchons donc à retirer un fichier de la zone d'index sans perdre les
modifications effectuées sur ce fichier.


## Mise en situation

* **Modifier 2 fichiers**: ``README.rst`` et ``default.css`` par exemple
* **git add .**: Ajoutez vos 2 modifications dans l'index (staging area)
* **git status**: constater que les 2 fichiers sont indexés

## Résolution

* **git reset README.md**: retire de l'index ``README.md``
* **git status**: constatez que seul le fichier ``default.css`` est indexé
* **git commit -m "modification de la feuille de style"**: commit le fichier
  indexé
