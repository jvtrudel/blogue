% Macport cookbook
% jvtrudel



# Nettoyage
    port clean --all all
http://superuser.com/questions/165652/how-can-i-clean-up-my-macports-installation


# configuration de python

    sudo port select --set python python34

    sudo port select --set ipython ipython34

    port select --set pip pip34

## obtenir la liste des groupes (utilisables avec _port select_)

    port echo '*_select' | cut -d_ -f1

## désactiver tous les libraries pythons 
  
    sudo port deactivate py-* and active



# Références

  - [Tâches courantes](https://guide.macports.org/chunked/using.common-tasks.html)


