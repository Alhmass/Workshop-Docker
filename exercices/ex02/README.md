# Exercice 2

L'objectif de cet exercice est d'orchestrer avec l'aide de docker compose différents services.

Le fichier docker-compose.yml doit contenir les choses suivantes :

* 3 services :
  -    Un serveur minecraft 1.14.2 :
        - Construisez l'image du premier exercice.
  -    Une base de donnée Mariadb :
          - Utiliser une image officielle Mariadb
          - Créez une base de données (nom au choix)
          - Créez un nouvel utilisateur
  -    Un site internet Wordpress :
          - Utiliser une image Wordpress PHP Apache existante
          - Rediriger le port 8080 de votre machine vers le port 80 du conteneur
 + 1 volume:
     - db-data qui doit permettre que les données de la base de données soit persistantes

## Bonus

* Mettre les variables d'environnement dans un fichier
* Utiliser docker secrets

