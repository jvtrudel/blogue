# Ressource

  - [The art of Linux programming](http://www.catb.org/esr/writings/taoup/html/)


# Administration système

## Gestion des utilisateurs

### Création d'utilisateurs

#### useradd

  - [documentation ubuntu](https://doc.ubuntu-fr.org/useradd)

### Inspecter les utilisateurs

  - [avec emphase sur utilisateurs avec privilèges *root* sur serverFault](http://serverfault.com/questions/208347/how-do-i-list-all-users-with-root)

### Détruire un compte utilisateur

  - [sur nixCraft](http://www.cyberciti.biz/faq/linux-remove-user-command/)

### Changer d'utilisateur dans le terminal

  - [sur unix stackexchange](http://unix.stackexchange.com/questions/3568/how-to-switch-between-users-on-one-terminal)

### Ajouter les permission sudo à la création d'un utilisateur
  - [sur ask ubuntu](http://askubuntu.com/questions/7477/how-can-i-add-a-new-user-as-sudoer-using-the-command-line)


Problème d'espace sur le disque /boot
-------------------------------------
Quand le "disque" /boot est plein, il peut y avoir des problèmes d'installation et de mise à jour avec apt-get et aptitude.
Linux conserve une image des versions précédentes. Pour les effacer:
1- Libérer de l'espace localement: sudo rm -rf /boot/*-3.2.0-{29,31,32,34,35}-*
2- Nettoyer un peu... sudo apt-get -f install
3- Effacer complètement les images disques: sudo apt-get purge linux-image-3.2.0-{29,31,32,34,35}*

[/boot disk management (forum)](http://askubuntu.com/questions/345588/what-is-the-safest-way-to-clean-up-boot-partition)

Machine et architecture
-----------------------
uname, lscpu


Permission
----------
[man page](http://www.computerhope.com/unix/uchmod.htm)


Groups
------
[wiki](https://wiki.archlinux.org/index.php/users_and_groups)

Shared Memory
-------------
[Use the command ipcs -lm to see the limit](http://www.rwitkop.com/VistA/ConfigureSysctl4Cache.html)

[ulimit -a ; ulimit -aH](https://groups.google.com/forum/?hl=fr#!searchin/gamess/max$20shared$20memory/gamess/XWmyMSfyKjU/Jy8OJ4lpybYJ)
