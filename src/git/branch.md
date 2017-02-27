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


## Travailler aevc des branches distantes

### Voir les branches distantes

    git branch -a

### cloner localement une branche distante

    git checkout -b local_branch_name origin/distant_branch_name


### [Intégrer une branche appartenant à un autre fork](http://stackoverflow.com/questions/14383212/git-pulling-a-branch-from-another-repository)

    git remote add fork <url of fork>
    git fetch fork
    git checkout -b fork_branch fork/<branch>

## Destruction d'une branche

### Destruction d'une branche locale

    git branch -d <branche à élaguer>

### Destruction d'une branche distante

    git push origin :<branche distante>

### Nettoyer localement les branches détruites sur le serveur d'attache

    git remote prune origin



## recombinaison et nettoyage de branches

### Rapatrier une branche de développement en nettoyant l'historique

On a deux branche **dev** et **master**

    git rebase -i master dev
    git checkout master
    git branch -d dev

## Astuces, bonnes pratiques et pièges à éviter

  - Réfléchir à vos choix de branche (utilité, objectif, lien avec les autres branches, ratio effort/avantage)
  - Attention à ne pas s'emmèler dans ses branches.
  - Une fonctionalité par branche
  - Utiliser les branches lorsque l'intégrité du master est critique (par exemple, pour un travail avec des collaborateurs).


## Ressources
