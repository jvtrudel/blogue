# Configuration
## Ajouter un mot de passe simple à la page (.htpasswd)

    # créer un utilisateur
    sudo sh -c "echo -n 'sammy:' >> /etc/nginx/.htpasswd"

    # ajouter le mot de passe
    sudo sh -c "openssl passwd -apr1 >> /etc/nginx/.htpasswd"

## Ajouter un certificat de sécurité SSL avec certbot/letsencrypt sur nginx

    certbot --nginx -d example.com -d www.example.com
