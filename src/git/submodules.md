# git submodule

## Importer les submodules d'un projet cloné

Lors du clonage d'un projet, les sous-projets ne sont pas importés automatiquement.

    git clone projet-incluant-submodules.git

Il faut le demander explicitement:

    git clone projet-incluant-submodules.git --recursive

Ou bien le demander par la suite:

    git clone projet-incluant-submodules.git
    git submodule init sobmodule
    git submodule update --remote


### Suivre une ou plusieurs branche à partir d'un submodule

## enlever un submodule d'un projet

En supprimant le répertoire locale:

    git submodule deinit un_submodule    
    git rm un_submodule

*attention: il ne faut pas laisser de slash à la fin de un_submodule*

En conservant le répertoire local:

    git rm --cached <asubmodule>
    rm -rf .git/modules/<asubmodule>


## webographie
  - [Documentation de la commande submodule](https://git-scm.com/docs/git-submodule)
  - [Using submodules in Git - Tutorial](http://www.vogella.com/tutorials/GitSubmodules/article.html)
  - [GETTING GIT SUBMODULE TO TRACK A BRANCH](http://www.activestate.com/blog/2014/05/getting-git-submodule-track-branch)
  - [What is the current way to remove a git submodule?](http://stackoverflow.com/questions/29850029/what-is-the-current-way-to-remove-a-git-submodule)
