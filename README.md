# Portfolio – Projet Trustia (3 exercices)

## 👤 Présentation du projet

Ce projet a été réalisé dans le cadre d’un exercice technique visant à mettre en place une application web complète conteneurisée. L’objectif principal est de maîtriser le déploiement d’une application Django connectée à une base de données PostgreSQL via Docker.

Le projet est structuré en **3 exercices progressifs**, permettant de comprendre étape par étape la mise en place d’un environnement de développement et de déploiement moderne.

---

## 🧩 Exercice 1 – Mise en place de l’environnement Docker

### 🎯 Objectif

Créer un environnement de développement reproductible avec Docker.

### ⚙️ Mise en œuvre

* Création d’un fichier `docker-compose.yml`
* Mise en place de deux services :

  * **db** : base de données PostgreSQL 15
  * **web** : application Django
* Configuration des variables d’environnement :

  * Nom de la base : `trustia`
  * Utilisateur : `trustia`
  * Mot de passe : `trustia`

### 📌 Résultat

Un environnement isolé permettant de lancer rapidement une base de données et une application web.

---

## 🧩 Exercice 2 – Développement de l’application Django

### 🎯 Objectif

Créer une application web fonctionnelle connectée à PostgreSQL.

### ⚙️ Mise en œuvre

* Initialisation du projet Django
* Configuration de la connexion à PostgreSQL
* Création des migrations :

  ```bash
  python manage.py migrate
  ```
* Lancement du serveur Django :

  ```bash
  python manage.py runserver 0.0.0.0:8000
  ```

### 📌 Résultat

Une application web accessible sur `http://localhost:8000` connectée à une base de données persistante.

---

## 🧩 Exercice 3 – Orchestration et automatisation

### 🎯 Objectif

Automatiser le déploiement complet de l’application.

### ⚙️ Mise en œuvre

* Utilisation de Docker Compose pour orchestrer les services
* Ajout de dépendances entre services (`depends_on`)
* Automatisation des migrations au démarrage :

  ```bash
  python manage.py migrate && python manage.py runserver
  ```
* Volume monté pour synchronisation du code :

  ```yaml
  volumes:
    - .:/app
  ```

### 📌 Résultat

Un déploiement automatisé en une seule commande :

```bash
docker compose up --build
```

---

## 🚀 Compétences acquises

* Docker & Docker Compose
* Déploiement d’applications web
* Django (backend Python)
* PostgreSQL
* Architecture micro-services simple
* Automatisation d’environnement de développement

---

## 📂 Lien du projet

🔗 [https://github.com/alexm-cell/trust_project](https://github.com/alexm-cell/trust_project)

---

## 🧠 Conclusion

Ce projet permet de comprendre la mise en place d’une architecture complète moderne basée sur la conteneurisation. Il constitue une base solide pour des projets plus avancés en DevOps et cybersécurité.
