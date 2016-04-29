# Supprimer les fichiers non suivis

Il arrive que votre application génère des fichiers dans le répertoire projet
(dans ce cas vous pourriez également envisager l'utilisation de `.gitignore`),
ou pour un tout autre raison...

Nous allons voir comment supprimer tous ces fichiers qui polluent notre répertoire
de travail

## mise en situation

* **touch fichier1**: création d'un nouveau fichier à la racine 
* **mkdir test**: création d'un répertoire de test
* **touch test/fichier2**: création d'un fichier dans le sous-répertoire
* **mkdir test2**: création d'un répertoire de test qui reste vide
* **modifier un fichier**: faire une modif dans un fichier pour constater
  qu'elle ne sera pas impactée
* **git status**: constatez les nouveaux fichiers non versionnés détectés par git
  (non ignoré par ``.gitignore``) et le fichier modifié


## résolution

* **git clean -n**: Afficher la liste des fichiers qui seront complètement
  supprimé du file système
* **git clean -n -d**: nous voullons également supprimer les répertoires
* **git clean -f -d**: **Attention cette commande est irréversible** supprime
  définitivement les fichiers non suivis par git
* **git status** / **tree** / **ls**: constatez que les fichier non suivis ont été
  supprimés et que les fichiers modifiés sont restés tels quels
