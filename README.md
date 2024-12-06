# Projet de Nettoyage et Analyse des Données Immobilières  

Ce projet vise à renforcer vos compétences en manipulation et analyse de données, modélisation statistique et application de techniques de machine learning pour résoudre des problèmes réels dans le domaine de l'immobilier.  

## Table des Matières  
- [Contexte du Projet](#contexte-du-projet)  
- [Objectifs](#objectifs)  
- [Tâches à Réaliser](#tâches-à-réaliser)  
  - [Connexion à la Base de Données](#connexion-à-la-base-de-données)  
  - [Exploration et Compréhension des Données](#exploration-et-compréhension-des-données)  
  - [Prétraitement des Données](#prétraitement-des-données)  
  - [Modélisation](#modélisation)  
    - [Régression Linéaire Multiple](#régression-linéaire-multiple)  
    - [Classification](#classification)  
  - [Analyse et Interprétation](#analyse-et-interprétation)  
  - [Visualisation des Résultats](#visualisation-des-résultats)  
  - [Amélioration des Modèles](#amélioration-des-modèles)  
- [Documentation et Reproductibilité](#documentation-et-reproductibilité)  
- [Réflexion sur les Biais et l'Éthique](#réflexion-sur-les-biais-et-léthique)  
- [Technologies Utilisées](#technologies-utilisées)  
- [Installation](#installation)  
- [Utilisation](#utilisation)  
- [Licence](#licence)  

## Contexte du Projet  
Le projet s'inscrit dans un cadre éducatif et a pour objectif d'explorer les données issues de l'immobilier tout en appliquant des techniques avancées de machine learning et de statistiques pour résoudre des problématiques concrètes.  

## Objectifs  
- Comprendre les relations entre les variables pour prédire les prix immobiliers.  
- Identifier les facteurs influençant la présence d’équipements spécifiques.  
- Fournir des recommandations basées sur des analyses de données fiables et reproductibles.  

## Tâches à Réaliser  

### Connexion à la Base de Données  
- Utiliser **SQLAlchemy** pour se connecter à une base de données PostgreSQL.  
- Importer les tables nécessaires : `Annonce`, `Ville`, `Équipement`, et `AnnonceEquipement`.  

### Exploration et Compréhension des Données  
- Examiner la structure des données et les relations entre les tables.  
- Identifier les variables clés pour les modèles de régression et de classification.  

### Prétraitement des Données  
1. **Gestion des valeurs manquantes** :  
   - Décider de la gestion des annonces avec un prix "PRIX NON SPÉCIFIÉ".  
2. **Transformation des variables** :  
   - Convertir les dates en composantes utiles (année, mois, jour).  
   - Encoder les variables catégorielles (`city_id`) avec des méthodes adaptées.  
   - Créer des variables binaires pour la présence ou l'absence d’équipements.  
3. **Normalisation/Standardisation** :  
   - Appliquer des transformations aux variables numériques si nécessaire.  

### Modélisation  

#### Régression Linéaire Multiple  
- **Sélection des Variables** : Identifier les variables pertinentes (e.g., `nb_rooms`, `surface_area`).  
- **Division des Données** : Séparer en ensembles d’entraînement (80%) et de test (20%).  
- **Entraînement et Évaluation** : Entraîner un modèle de régression linéaire et évaluer sa performance (MSE, R²).  

#### Classification  
- **Création de la Variable Cible** : Identifier la présence d’un équipement (e.g., ascenseur).  
- **Gestion du Déséquilibre des Classes** : Utiliser des techniques comme SMOTE si nécessaire.  
- **Entraînement de Modèles** : Tester plusieurs algorithmes (régression logistique, arbres de décision, etc.).  
- **Évaluation** : Comparer les performances des modèles avec des métriques comme le score F1 et l’AUC-ROC.  

### Analyse et Interprétation  
- Interpréter les coefficients du modèle de régression.  
- Analyser la matrice de confusion et l’importance des variables pour les modèles de classification.  

### Visualisation des Résultats  
- Créer des graphiques exploratoires (histogrammes, corrélations).  
- Visualiser les courbes ROC et les graphiques des résidus.  

### Amélioration des Modèles  
- **Feature Engineering Avancé** : Ajouter des interactions ou des variables polynomiales.  
- **Optimisation des Hyperparamètres** : Utiliser des techniques comme Grid Search.  

## Documentation et Reproductibilité  
- Commentez chaque étape de votre code.  
- Fournissez un rapport détaillé et un fichier `README` clair pour guider les utilisateurs.  

## Réflexion sur les Biais et l'Éthique  
- Identifier les biais dans les données et leur impact sur les modèles.  
- Réfléchir aux implications éthiques de l’utilisation des modèles dans un contexte réel.  

## Technologies Utilisées  
- **Python** : Pandas, NumPy, Matplotlib, Scikit-learn  
- **SQLAlchemy** : Connexion à PostgreSQL  
- **PostgreSQL** : Gestion de la base de données  
- **Docker** : Environnement conteneurisé  

## Installation  
1. Clonez le dépôt :  
   ```bash  
   git clone "coupier le lien ssh ou ..."
