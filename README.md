# WORKSHOP EPITECH -> Découverte Flask

Bienvenue dans le Workshop EPITECH sur la découverte de Flask ! Ce guide vous aidera à explorer Flask en profondeur tout en abordant des sujets avancés.

## Table des Matières

1. [Introduction -- 5 min](#introduction)
2. [Les Bases de Flask -- 45 min / 1h](#bases)
3. [Gestion des Fichiers -- 45 min](#gestion)
4. [Authentification et Sécurité -- 1h](#security)

## Introduction (MAX 10 MIN / ABSENT)

Dans cette première section, nous mettrons en place notre environnement de développement Flask.

### Installation de Flask (Prérequis)

- Installez Flask en utilisant pip.
- Créez un environnement virtuel pour votre projet Flask.

### Créez un Projet de Base

- Créez un répertoire pour votre projet Flask.
- Initialisez un fichier Python (app.py) pour votre application web.

## Les Bases de Flask (45 min / 1h)

Dans cette section, nous explorerons les fondamentaux de Flask.

### Gestion des Routes Complexes

- Dans le fichier app.py, créez une route /hello/<name> qui affiche un message de salutation personnalisé en utilisant le paramètre name.
- Testez cette route en ouvrant votre navigateur et en accédant à http://localhost:5000/hello/votre-nom.


### Blueprints

- Créez un blueprint nommé auth dans un fichier séparé.
- Ajoutez une route /login à ce blueprint qui affiche un formulaire de connexion.
- Utilisez le blueprint dans votre application principale pour gérer les routes liées à l'authentification.
- Testez la route /login en vous rendant sur http://localhost:5000/auth/login.


### Utilisation de Cookies et de Sessions

- Ajoutez la prise en charge des sessions dans votre application Flask.
- Créez une route /login qui stocke un identifiant de session lorsque l'utilisateur se connecte.
- Créez une route /logout qui supprime l'identifiant de session lorsque l'utilisateur se déconnecte.

## Gestion des Fichiers (45 min)

Dans cette section, nous aborderons la gestion des fichiers avec Flask.

### Téléchargement de Fichiers

- Créez une route /upload qui permet aux utilisateurs de télécharger des fichiers.
- Utilisez Flask-Uploads pour gérer les téléchargements de fichiers.
- Affichez un message de succès après le téléchargement du fichier.

### Génération de Fichiers PDF

- Installez la bibliothèque ReportLab en utilisant pip.
- Créez une route /generate-pdf qui génère un fichier PDF simple en utilisant ReportLab.
- Servez le fichier PDF généré en tant que réponse HTTP.
  
## Authentification et Sécurité (45 min)

Dans cette section, nous nous concentrerons sur la sécurité de votre application Flask.

### Authentification par Token

- Utilisez la bibliothèque Flask-JWT-Extended pour implémenter l'authentification basée sur les tokens.
- Créez une route /protected qui nécessite un token valide pour accéder.

### Protection contre les Attaques CSRF

- Utilisez Flask-WTF pour ajouter une protection CSRF à votre formulaire de connexion.
- Vérifiez que votre application rejette les soumissions de formulaire CSRF.


