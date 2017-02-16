% Comment gérer un serveur web pour un usage local




# Intro
Contrairement au développement html/css pour lequel il suffit simplement d'ouvrir le fichier index.html dans avec votre navigateur web favori, l'affichage d'une page web en php demande d'être interprété par un serveur web. Il est possible, surtout à l'étape du dévelloppement, de faire ceci directement sur votre ordinateur. Cela nécessitera l'installation d'apache et, possiblement, de mysql.

# Apache

## insatller

## configurer
Dans /etc/apache2
Fichier de configuration: httpd.conf

## lancement du serveur
    sudo launchctl start apache2
    sudo launchctl stop apache2


## localisation de apache (fichiers de configurations)
répertoire:    /private/etc/apache2


# On fait simple: répertoire par défaut
Répertoire par défault






# On fait compliqué: masque dns  dnsmasq 
Fichiser de configuration: /opt/local/etc/dnsmasq.conf



# liste exhaustive
Mais non compréhensible de tous les fichiers et répertoires en lien avec la configuration

  - /private/etc/hosts
  - /etc/resolver/dev 
  - /etc/apache2/users/
  - /private/etc/apache2/httpd.conf
  - /private/etc/apache2/extra/httpd-vhosts.conf







# Références

[Solution](http://coolestguidesontheplanet.com/get-apache-mysql-php-phpmyadmin-working-osx-10-10-yosemite/)

[Configuration élémentaire](http://osxdaily.com/2012/09/02/start-apache-web-server-mac-os-x/)

[Général](http://mallinson.ca/osx-web-development/)

[macsox+php+mysql](http://elliptips.info/installer-apache-mysql-et-php-sous-osx-sans-passer-par-mamp/)

[masque dnsmasq1](http://www.42umbrellas.com/2012/08/14/setting-up-deevelopment-shop-on-osx-mountain-lion/)

[masque dnsmasq2](https://www.computersnyou.com/3786/how-to-setup-dnsmasq-local-dns/)

[masque dnsmasq3](http://passingcuriosity.com/2013/dnsmasq-dev-osx/)

[mysql](https://trac.macports.org/wiki/howto/MySQL)



