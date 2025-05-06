
- **Le reverse proxy** est le seul point d'entrée. Il redirige le trafic :
  - vers le **serveur front-end** pour le contenu statique
  - vers l’un des **serveurs API** via un algorithme de **Round Robin**

---

## ⚖️ Qu’est-ce que le Round Robin Load Balancing ?

Le Round Robin est une méthode de répartition du trafic réseau où chaque serveur reçoit les requêtes à tour de rôle.  
Exemple avec 3 serveurs A, B et C :

1. Requête 1 → A  
2. Requête 2 → B  
3. Requête 3 → C  
4. Requête 4 → A  
...

Ce système est simple, efficace, et suffisant pour notre cas d'apprentissage.

---

## 🧰 Pré-requis

- Docker Desktop installé sur votre machine locale :  
  👉 https://www.docker.com/

- Environnement recommandé : **Windows**, **macOS**, ou **Linux**

- 📚 Ressources utiles :
  - [Docker Tutorial (officiel)](https://docs.docker.com/get-started/)
  - [Docker Cheatsheet](https://github.com/wsargent/docker-cheat-sheet)
  - [Proxy vs Reverse Proxy (vidéo YouTube – jusqu’à 06:25)](https://www.youtube.com/watch?v=7-LrdKJxqG8)

---

## 🚀 Objectifs du Projet

- Créer une application multi-conteneurs avec :
  - Reverse proxy + Load balancer (via Nginx par ex.)
  - 2 conteneurs pour les serveurs d’API
  - 1 conteneur pour le serveur front-end
- Mettre en place la communication entre les conteneurs
- Utiliser Docker Compose pour orchestrer les services

---

## 📦 À venir

- Structure du projet
- Fichiers Dockerfile pour chaque service
- Configuration du reverse proxy avec Nginx
- Fichier `docker-compose.yml`

---

## ✅ À la fin de ce projet, vous aurez appris à :

- Concevoir une architecture microservices simple avec Docker
- Mettre en œuvre un reverse proxy et un load balancer
- Utiliser Docker Compose pour gérer plusieurs conteneurs
- Appliquer une stratégie de répartition de charge basique

---