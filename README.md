# 📚 Application Bibliothèque (Node.js + Express + PostgreSQL)

<img width="1237" height="890" alt="image" src="https://github.com/user-attachments/assets/a8bfdc73-7de8-4934-9f26-74957b0de6f1" />

## 📖 Description

Cette application est un système de gestion de bibliothèque permettant de gérer :

* Les **auteurs**
* Les **livres**
* Les relations entre auteurs et livres

Elle utilise :

* **Node.js** avec **Express**
* **PostgreSQL** pour la base de données
* **EJS** comme moteur de templates

---

## 🚀 Installation

### 1. Cloner ou créer le projet

```bash
mkdir bibliotheque-app
cd bibliotheque-app
```

### 2. Initialiser le projet

```bash
npm init -y
```

### 3. Installer les dépendances

```bash
npm install
```

---

## 📦 Dépendances principales

* express
* ejs
* pg
* dotenv

### Dépendance de développement

* nodemon

---

## 📁 Structure du projet

```
bibliotheque-app/
├── config/
├── controllers/
├── models/
├── routes/
├── views/
│   ├── partials/
│   └── pages/
├── public/
├── .env
├── app.js
└── package.json
```

---

## ⚙️ Configuration

Créer un fichier `.env` à la racine du projet :

```
DB_USER=utilisateur
DB_PASSWORD=mot_de_passe
DB_HOST=localhost
DB_PORT=5432
DB_DATABASE=bibliotheque_db
PORT=3000
```

---

## 🗄️ Base de données

1. Créer la base PostgreSQL :

```
bibliotheque_db
```

2. Créer les tables :

* auteurs
* livres

3. Ajouter des données de test (optionnel)

---

## ▶️ Lancer le projet

### Mode développement (recommandé)

Ajouter dans `package.json` :

```json
"scripts": {
  "dev": "nodemon app.js"
}
```

Puis lancer :

```bash
npm run dev
```

### Mode normal

```bash
node app.js
```

---

## 🌐 Accès à l'application

Ouvrir dans le navigateur :

```
http://localhost:3000
```

---

## 🧩 Fonctionnalités

### 📌 Auteurs

* Liste des auteurs
* Ajouter un auteur
* Modifier un auteur
* Supprimer un auteur
* Voir les détails + livres associés

### 📚 Livres

* Liste des livres
* Recherche de livres
* Ajouter un livre
* Modifier un livre
* Supprimer un livre
* Voir les détails

---

## 🔍 Recherche

Recherche de livres par :

* Titre
* Nom de l’auteur
* Genre

---

## 🎨 Frontend

* Templates avec **EJS**
* Fichiers statiques dans `/public`

  * CSS
  * JavaScript

---

## ❗ Erreurs gérées

* Page 404
* Gestion des erreurs serveur

---

## 🛠️ Améliorations possibles

* Authentification utilisateur
* Pagination
* API REST
* Upload d’images
* Dashboard admin

