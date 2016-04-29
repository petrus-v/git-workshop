# Travailler avec plusieurs remotes

> **TODO**: Ajouter une illustration

* **Forker le repo github**: Faire les manipulations sous github!
* **git remote add <votrepseudo> git@github.com/<pseudo>/git-workshop-example**:
  Référence un nouveau répertoire distant (repo)
* **git fetch <pseudo>**: Rapatrie les information du repo distant
* **git push <pseudo> <votrenom>**: pousser votre branche sur votre repo distant
* **git push <pseudo> <votrenom>-1.0**: pousser le tag sur votre repo distant
* **git remote**: visualiser les remotes
* **git remote -v**: afficher les urls fetch/push utilisé pour chaque nom de
  repo
* **git branch**: affiche uniquement les branche du repo courant
* **git branch -a**: affiche également les branches des repos distants
* **git branch -a -v**: affiche le commit pointé par la branche
* **git branch -a -vv**: ajoute l'upstream de la branche
* **git branch --set-upstream-to=<pseudo>/<votrenom> <votrenom>**: définit
  l'upstream de votre branche.
