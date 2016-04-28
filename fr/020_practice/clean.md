# Supprimer les fichiers non suivi

Il arrive que votre application génère des fichier dans le répertoire projet
(dans ce cas vous pourriez également envisager l'utilisation de `.gitignore`),
ou pour un tout autre raison...

Nous allons voir comment supprimer tous ces fichier qui pollue notre répertoire
de travail

## mise en situation

* **touch fichier1**: création d'un nouveau fichier à la racine 
* **mkdir test**: création d'un répertoire de test
* **touch test/fichier2**: création d'un fichier dans le sous répertoire
* **mkdir test2**: création d'un répertoire de test qui reste vide
* **modifier un fichier**: faire une modif dans un fichier pour constater
  qu'elle ne sera pas impacté
* **git status**: constaté les nouveaux fichiers non versionné détecté par git
  (non ignoré par ``.gitignore``) et le fichier modifié


## résolution

* **git clean -n**: Afficher la liste des fichiers qui seront complètement
  supprimé du file système
* **git clean -n -d**: nous voullons également supprimer les répertoires
* **git clean -f -d**: **Attention cette commande est irréversible** supprime
  définitivement les fichiers non suivi par git
* **git status** / **tree** / **ls**: constaté que les fichier non suivi ont été
  supprimé et que les fichiers modifié sont resté tel quels
