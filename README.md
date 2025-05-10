# Gestion des Posts

## Fonctionnalités
- Création, modification et suppression de posts.
- Gestion des utilisateurs avec authentification.
- Recherche et filtrage des posts.
- Pagination des résultats.
- API RESTful pour l'intégration avec des clients externes.

## 🚀 Technologies utilisées
- **Backend** : Node.js, Express.js
- **Base de données** : MongoDB
- **Authentification** : JSON Web Tokens (JWT)
- **Autres** : dotenv, bcrypt

## 📦 Structure du projet

Voici une description détaillée de la structure du projet pour vous aider à naviguer dans le code :

```
/Gestion des Posts  
├── /controllers  
│   ├── authController.js       # Gère les opérations liées à l'authentification et aux autorisations.  
│   ├── postsController.js      # Gère les opérations CRUD (Créer, Lire, Mettre à jour, Supprimer) pour les posts.  
│  
├── /middlewares  
│   ├── identification.js       # Middleware pour vérifier les jetons JWT et sécuriser les routes.  
│   ├── validator.js            # Middleware pour valider les données des requêtes entrantes.  
│  
├── /models  
│   ├── postsModel.js           # Définition du schéma Mongoose pour les posts.  
│   ├── usersModel.js           # Définition du schéma Mongoose pour les utilisateurs.  
│  
├── /routes  
│   ├── authRoutes.js           # Définit les routes API pour les opérations d'authentification.  
│   ├── postRoutes.js           # Définit les routes API pour les opérations sur les posts.  
│  
├── /utils  
│   └── hashing.js              # Contient des fonctions utilitaires pour le hachage des mots de passe.  

└── index.js                    # Point d'entrée principal de l'application, configure et lance le serveur Express.  
├── package.json                # Fichier listant les dépendances et scripts du projet.  
├── package-lock.json           # Fichier de verrouillage des dépendances pour garantir des versions cohérentes.  
├── requests.rest               # Fichier pour tester les requêtes API avec des outils comme REST Client.  

```

Chaque dossier et fichier a un rôle spécifique pour assurer une organisation claire et une maintenance facile du projet.

## Installation
1. Clonez le dépôt :
    ```bash
    git clone https://github.com/Abderrazzak10/Gestion-des-Posts.git
    ```
2. Installez les dépendances :
    ```bash
    npm install
    ```
3. Configurez les variables d'environnement dans un fichier `.env`.

## Lancement
- En mode développement :
  ```bash
  npm run dev
  ```
## Licence
Ce projet est sous licence MIT.