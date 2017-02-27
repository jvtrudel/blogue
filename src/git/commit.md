# Exemples d'utilisation

## Faire un commit et le commenter

    git commit -m "mon commentaire doit être utile"

## Commentaire détaillé incluant sujet et un développement

    git commit -m "sujet de mon commit" -m "paragraphe 1" -m "paragraphe 2 " -m " ... "

## Passer en mode éditeur texte pour

    git commit

Pour configurer votre éditeur par défault (et ne pas vous retrouver avec vi ou nano):

    git config --global core.editor votre_editeur_texte_favori

## Commiter tout en ajoutant toutes les modifications

    git commit -am "Fin de journée. J'en ai mare, je sauvegarde tout et je nettoierai plus tard..."

    git commit --all

**Attention**: ceci ne marche pas pour les fichiers qui n'ont pas été mis à l'index (````git add````).

# Explication de la commande commit


# WebOgraphie

  - [git commit. Par: git-scm](https://git-scm.com/docs/git-commit)
  - [how to write a commit message. Par: Chris Beams ](http://chris.beams.io/posts/git-commit/)
