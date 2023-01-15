
# Projet Docker

Ce projet d'école est pour but de comprendre comment utiliser le Docker Compose et créer des images avec le Dockerfile en mettrant en place :

* Deux services Nginx
* Deux services PHP (Laravel)
* Une base de données MYSQL
* D'autres services supplémentaires : un serveur Minecraft, un outil de gestion de BDD : Adminer, un serveur de stockage : Minio

## Déploiement

Afin de déployer ce projet :

* Exécuter `docker compose build --pull --no-cache` pour créer des nouvelles images
* Vérifier le fichier `script.sh`, remplacer `#!/bin/bash` (windows par défault) par `#!/usr/bin/env bash`si vous êtes sur macOS ou `#!/usr/bin/bash`si vous êtes sur Linux 
* Exécuter `./script.sh` pour démarrer les services et exécuter les commandes de démarrage de Laravel
* Ouvrir `https://localhost:80`ou `https://localhost:81` sur un navigateur web pour accéder aux services web PHP
* Exécuter `docker compose down --remove-orphans`pour arrêter les conteneurs Docker