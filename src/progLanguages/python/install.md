

# Options setuptools

## Pour l'installation de version de développement

(Voir l'explication de cette recette](http://stackoverflow.com/questions/19048732/python-setup-py-develop-vs-install)

    python setup.py develop

Utiliser setuptools (et develop!) avec un setup.py qui ne le contient pas...

    sudo python -c "import setuptools;exec(open('setup.py').read())" develop
    


## Désistallation

on doit dabord créer la liste des fichiers installés. puis, les suprimer avec la commande xargs:

    sudo python setup.py install --record files.txt
    cat files.txt | sudo xargs rm -rf


# Avec pip

Utiliser pip pour bénéficier des fonctionalités de pipy

[Voir ce bidouillage stackexchange](http://stackoverflow.com/questions/1900775/how-to-have-pip-install-editable-to-run-sdist-instead-of-develop)
[Etce bidouillage là aussi](http://stackoverflow.com/questions/15031694/installing-python-packages-from-local-file-system-folder-with-pip)



