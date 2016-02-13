# Branches

  - Les branches servent à faire des développement sans toucher à la branche principale. 

  - Permet de focuser son attention sur le dévellopement d'une fonctionalité.
  - Permet de mener des dévelloppements en parallèle.  


Voir également les sections suivantes:

  - merge

## Création d'une branche

### Création rapide 

    git checkout -b <nom de la nouvelle branche>

### Spécification de la branche d'ancrage

    git checkout -b <fonctionnalité> <branche parent>

### Synchronisation avec un serveur distant

    git push --set-upstream origin <nom de la branche à mettre sur le serveur>

### Inspection des branches distantes

    git remote show origin

## Destruction d'une branche

### Destruction d'une branche locale

    git branch -d <branche à élaguer>

### Destruction d'une branche distante

    git push origin :<branche distante>

### Nettoyer localement les branches détruites sur le serveur d'attache

    git remote prune origin







## Astuces, bonnes pratiques et pièges à éviter

  - Réfléchir à vos choix de branche (utilité, objectif, lien avec les autres branches, ratio effort/avantage)
  - Attention à ne pas s'emmèler dans ses branches.
  - Une fonctionalité par branche
  - Utiliser les branches lorsque l'intégrité du master est critique (par exemple, pour un travail avec des collaborateurs).


## Ressources 
