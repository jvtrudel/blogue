tags: "openIdConnect"

---
# Devenez fournisseur d'identidé

Résumé

## Les irritants de la

Tout développeur web a un jour où l'autre, si ce n'est pas à sa première journée de travail à concevoir un système d'authentification des utilisateurs. Ceci n'est pas très compliqué, néanmoins, formulaire de login, gérer et assurer la sécurité des mots de passes et des données personnels, interface de gestion des données personnels, mécanisme de récupération de mot de passe oubliés, etc... etc. Ceci n'est pas très compliqué, mais il faut le faire et, si vous êtes le moindrement respectueux des utilisateurs et de leurs données, vous voudrez le faire bien!

Or, cette activité (création de compte utilisateurs) est tellement routinière dans le domaine du service web que l'on a rapidement cherché à trouver une solution moins laborieuse. [SAML, 2001](https://en.wikipedia.org/wiki/Security_Assertion_Markup_Language), [Oauth, 2006](https://en.wikipedia.org/wiki/OAuth), [Oauth2, ]

Aujourd'hui, tous les gros joueurs ( [twitter](https://dev.twitter.com/web/sign-in), [google](https://developers.google.com/identity/protocols/OpenIDConnect), facebook, github, ...) utilisent OAuth2 pour leur processus d'autorisation et offre également des services de fournisseur d'identité. Ce fameux sign-in with ... qui nous facilite tant la vie.

(pour savoir si vous avez vraiment besoin d'un )


## La tendance de l'heure en maitère d'authentification/autorisation

Oaunt2 + JWT = openID connect

openID connect émerge comme étant la solution la plus sécuritaire, ouverte et la plus répandue. Consortium d el'industrie et s'implante tranquillement dans le domaine gouvernemental, recommandé par ... gouv québec.

## Pourquoi se contenter d'être client?

La solution la plus simple est certainement d'externaliser complètement les services d'autorisation auprès des grands fournisseurs. Plus de mot de passe à gérer, plus de ... Il suffit d'avoir un compte github ou snapchat, et le tour est joué! on n'aura aucun nouveau mot de passe à se remémorer.


Cette solution est idéale si l'information que vous stocké ou que vous transigée est peu importante. Mais dans des cas plus stratégiques (pour des affaires gouvernementales ou en entreprise), il devient plus délicat d'impliquer une tierce partie. Même s'il y a très peu de risques du point de vue de la sécuriét, le rapport de confiance devient primordial et il n'est pas déraisonnable de vouloir rester le seul maitre à bord de ses affaires.

## Mettre en place un service ID Provider

Une solution intéressante pour une entreprise, une institution ou un fournisseur de plusieurs services web est de mettre en place. En plus d'être tendance et branché, cela vous positionne parmi les joueurs sérieux.

### À même le service

self-issued

### En tant qu' API


## Offrez vos service via openId connect

Votre serveur du grand public, mais il



Vous pouvez consulter d'autres articles de moi pour plus de renseignement sur [les services en ligne] ou pour apprendre comment [mettre en place un API Restful pour l'autorisation d'identité].

# Quelques mise en garde

  - pas autorisation, ni authentificaiton, mais pour delegation!


# Ressources
  - [Spécificaitons de l'openID connect](http://openid.net/connect/)
  - [Très bonne explicaiton de open ID connect par connect2id](http://connect2id.com/learn/openid-connect)
  - [Comment batir un service ID Provider, IBM](https://www.ng.bluemix.net/docs/services/mobileaccess/custom-auth-identity-provider.html)
  - [API security, oauth and openID connect by nordic APIs]
(http://nordicapis.com/api-security-oauth-openid-connect-depth/)

 pour l'ensemble de ses services
