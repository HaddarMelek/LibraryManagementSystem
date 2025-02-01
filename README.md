# Library Manager

## Description
**Library Management System** est une application web développée avec **ReactJS** pour le frontend et **NodeJS** pour le backend. Cette application permet la gestion des livres d'une bibliothèque, notamment leur émission, leur retour et leur consultation.

## Technologies utilisées
- **Frontend** : ReactJS
- **Backend** : NodeJS
- **Base de données** : MySQL (via XAMPP pour le serveur local)
- **Gestion des processus** : Concurrently

## Installation et exécution
1. **Cloner le projet** :
   ```bash
   git clone https://github.com/HaddarMelek/LibraryManagementSystem.git
   cd LibraryManagementSystem
   ```
2. **Installation des dépendances** :
   - Pour le frontend :
     ```bash
     cd frontend
     npm install
     ```
   - Pour le backend :
     ```bash
     cd ../backend
     npm install
     ```
3. **Démarrer l'application** :
   ```bash
   npm run dev
   ```
   > L'application frontend et le serveur backend seront lancés simultanément grâce à `concurrently`.

## Base de données
Le projet utilise une base de données **MySQL** nommée `library`. La base de données ainsi que les tables sont créées automatiquement, mais les données initiales des étudiants et des livres doivent être insérées manuellement.

### Tables principales
- **book** : Contient les informations des livres disponibles.
- **student** : Stocke les données des étudiants.
- **borrow** : Enregistre les emprunts de livres par les étudiants.

## Fonctionnalités principales
### Backend (NodeJS)
- **createDB** : Crée la base de données si elle n'existe pas.
- **createTables** : Génère les tables nécessaires.
- **credentials** : Contient les identifiants de connexion MySQL (penser à ajouter le mot de passe dans `credentials.js`).

### Frontend (ReactJS)
- **Books** : Affiche la liste des livres disponibles.
- **Issue** : Permet d'émettre un livre pour un étudiant.
- **Return** : Affiche la liste des livres empruntés et propose une option de retour.
- **Search** : Recherche les étudiants ayant emprunté un livre donné.
- **Nav** : Barre de navigation de l'application.

