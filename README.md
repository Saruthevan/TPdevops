Repo : https://github.com/Saruthevan/TPdevops.git

L’objectif de ce projet est de mettre en place une CI permettant de préparer une mise en production Kubernetes à partir d’un docker-compose existant.
Dans ce projet, j’ai mis en place une pipeline CI avec GitHub Actions qui fait les étapes suivantes :
    
Récupération du code du dépôt
Installation de Kompose
Génération automatique des manifestes Kubernetes (Deployment, Service, Secret) à partir du docker-compose.yaml
Regroupement des fichiers Kubernetes dans un dossier
Création d’un zip de rendu
Envoi automatique de ce zip sur un serveur FTP

Les secrets utilisés dans le projet (FTP et MariaDB) sont configurés dans GitHub Actions (Repository Secrets)
