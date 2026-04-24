# 🚀 Trustia Project

## 📌 Présentation

Trustia est une application web simple basée sur Django et PostgreSQL, entièrement conteneurisée avec Docker.

Le projet permet de mettre en place rapidement un environnement de développement reproductible pour une application web connectée à une base de données.

---

## 🧱 Architecture

Le projet est composé de deux services principaux :

* Une base de données PostgreSQL 15 utilisée pour stocker les données de l’application
* Une application web développée avec le framework Django

Ces deux services communiquent entre eux grâce à Docker Compose.

---

## ⚙️ Fonctionnement du projet

Au lancement, l’environnement démarre automatiquement :

* La base de données PostgreSQL est initialisée
* L’application Django se connecte à la base de données
* Les migrations sont appliquées pour créer les tables nécessaires
* Le serveur web Django devient accessible via un navigateur

---

## 🧠 Objectif du projet

Ce projet a pour but de démontrer la mise en place d’une architecture web moderne basée sur :

* Le développement backend avec Django
* L’utilisation d’une base de données relationnelle PostgreSQL
* La conteneurisation avec Docker
* L’orchestration de services avec Docker Compose

---

## 🚀 Résumé

* Application web Django
* Base de données PostgreSQL
* Environnement entièrement conteneurisé
* Architecture simple et reproductible

---

## 👤 Auteur

Alexandre Messein
GitHub : [https://github.com/alexm-cell](https://github.com/alexm-cell)
