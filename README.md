# Softy-Pinko Docker Project

Ce projet démontre l'utilisation de Docker pour créer une infrastructure web avec un reverse proxy, un équilibrage de charge, plusieurs serveurs API et un serveur front-end. L'objectif est de containeriser et orchestrer plusieurs services en utilisant Docker et Docker Compose.

## Aperçu du projet

Dans ce projet, vous containerisez une application qui comprend :
- Un **serveur proxy** utilisant Nginx, qui route le trafic entre les serveurs API et le serveur front-end.
- **Deux serveurs API** qui renvoient des données dynamiques, équilibrés via un algorithme round-robin.
- Un **serveur front-end** qui sert du contenu statique et consomme l'API pour les données dynamiques.

## Fonctionnalités

- **Services containerisés** : Docker est utilisé pour créer des environnements isolés pour le front-end et les back-end.
- **Équilibrage de charge** : Le trafic est distribué entre plusieurs serveurs API.
- **Docker Compose** : Facilite l'orchestration de l'application multi-conteneur.
- **Scalabilité** : Possibilité d'ajouter facilement plusieurs instances de serveurs API pour gérer une montée en charge.

## Structure des fichiers

- **Task 0** : Créer une première image Docker qui affiche "Hello, World!".
- **Task 1** : Serveur API backend utilisant Flask.
- **Task 2** : Serveur front-end utilisant Nginx.
- **Task 3** : Connexion entre le front-end et le back-end avec des appels AJAX.
- **Task 4** : Utilisation de Docker Compose pour orchestrer les services.
- **Task 5** : Mise en place d'un serveur proxy Nginx pour router le trafic.
- **Task 6** : Scalabilité horizontale avec plusieurs serveurs API.

## Comment exécuter le projet

1. **Cloner le dépôt** :

   ```bash
   git clone https://github.com/holbertonschool-softy-pinko-docker.git
   cd holbertonschool-softy-pinko-docker
