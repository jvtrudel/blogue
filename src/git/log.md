# historique (log)

## Nettoyage de l'historique avec rebase

Utiliser rebase en mode interactif:

    git rebase -i

Dans le fichier vim, on assigne une action à appliquer à chaque commit.

Pour restreindre le nombre (*n=1,2,3...*) de commit à rebaser:

    git rebase -i HEAD~n
