
# Copier d'un projet existant Fork

## Utilitée d'un fork

## Comment fonctionne un fork

## Fork cookbook

### Synchroniser un projet que l'on a forké

[blogue](http://www.croes.org/gerald/blog/synchroniser-son-fork-github-avec-le-projet-original/551/)
[github doc](https://help.github.com/articles/syncing-a-fork/)

    #Ajoutez à votre fork le remote du projet d'origine
    $ git remote add projet_original_master git://github.com/repo/projet_original.git

    #Mettez à jour votre fork en local
    $ git fetch projet_original_master

    #Fusionnez (merge) maintenant votre copie locale 
    # avec le projet d'origine
    $ git checkout master
    $ git merge projet_original_master/master

    #Validez vos changements
    $ git commit -a -m "Synchronisation avec le projet original"

    #Envoyez vos changements sur github
    $ git push

