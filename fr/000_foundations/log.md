# Voir l'historique des commits


* **git checkout <votrenom>**: on se positionne sur la branche <votrenom>
* **git log**: affiche la liste des commits sur la branche courante
* **git log --oneline**: version condensé d'u commit sur une ligne
* **git log --oneline --graph**: version condensé des commits sur une ligne
* **git log --oneline --graph --decorate**: ajoute les informations de branches,
  tags, HEAD
* **git log --oneline --graph --decorate --all**: ajoute les branches non 
  mergées
* **git log --stat**: Pour connaître les fichiers modifié par commits
* **git log --patch**: pour voir les changement effectué par commits

> **Note**: Possibilité de faire des aliais avec git.

Configuration de l'alias

```bash
$ git config --global alias.l "log --oneline --graph --decorate"
```

Utilisation de l'alias
```bash
$ git checkout master
Basculement sur la branche 'master'
Votre branche est à jour avec 'origin/master'.

$ git l
* fddbe2c (HEAD, origin/master, master) add content
* 94352b3 Add basic style
* 4af54b7 add content
* 9236e15 Initial commit

$ git l --all
* c81c1c2 (tag: pierre-1.0, pierre) add LICENSE and contact
* 984d372 add author
* fddbe2c (HEAD, origin/master, master) add content
| * 4edc386 (origin/feature-advanced-style, feature-advanced-style) Nice style
|/  
* 94352b3 Add basic style
* 4af54b7 add content
* 9236e15 Initial commit
```

> **Note**: Vous aurez remarqueé que vous pouvez toujours ajouter les
> paramètres à la suite
