# FIT YOUR BOOTY

Application web permettant de suivre ses données personnelles  nutritionnelles, sportives, et de santé. 

Site en production : [https://fit.vatinel.fr] 

! Création de compte soumis à procédure Auth ! 

!! Destiné à utilisation privée le site en production ne respecte pas la reglementation RGPD (clonez plutôt le repo) !! 


### L'application se divise en trois onglets
* Nutrition & Neat : Suivi des calories, macro, poids, steps, dépense énergétique
     répartie en 3 cards :
    
              - formulaire d'entrée des données
              - graphique plotly pour le suivi chronologique des métriques
              - tableau récapitulatif des entrées avec possibilité de modification


* Sport  : Suivi des séances de sport cardio / musculation.
              
            - choix des séances / exercices / métriques.
            - graphique plotly pour le suivi chronologique des métriques selon plusieurs aggrégations.
            - administration des exercices et des séances (créations personnalisables).
  
* Santé  : Suivi de marqueurs biologiques d'analyse sanguine.
  
          - formulaire d'entrée des données
          - tableau d'édition des analyses enregistrées
          - graphique plotly pour le suivi chronologique des marqueurs


## Aperçu de l'application

> Les captures ci-dessous utilisent exclusivement des données fictives créées pour la démonstration.

### Nutrition, NEAT et suivi du poids

<p align="center">
  <img src="docs/screenshots/dashboard-overview.png" alt="Vue générale du tableau de bord avec des données fictives" width="49%">
  <img src="docs/screenshots/dashboard-analytics.png" alt="Graphiques de suivi nutritionnel avec des données fictives" width="49%">
</p>

### Activité sportive

<p align="center">
  <img src="docs/screenshots/activity-overview.png" alt="Historique fictif des séances sportives" width="49%">
  <img src="docs/screenshots/activity-analytics.png" alt="Graphique fictif de progression sportive" width="49%">
</p>

### Suivi biologique

<p align="center">
  <img src="docs/screenshots/biology-overview.png" alt="Vue générale du suivi biologique avec des données fictives" width="49%">
  <img src="docs/screenshots/biology-analytics.png" alt="Courbe biologique construite avec des données fictives" width="49%">
</p>

### Version mobile

<p align="center">
  <img src="docs/screenshots/dashboard-mobile.png" alt="Version mobile du tableau de bord" width="390">
</p>



Le projet est déployé sur un **VPS Linux** et le code est versionné via **GitHub**.

---

# Stack technique

* Laravel
* PHP 8+
* MySQL / MariaDB
* JavaScript
* Plotly.js
* Git / GitHub
* VPS Linux (Ubuntu)

---

# Installation locale

Cloner le projet :

```
git clone git@github.com:SebV-code/FitYourBooty.git
cd FitYourBooty
```

Installer les dépendances :

```
composer install
```

Créer le fichier `.env` :

```
cp .env.example .env
```

Générer la clé Laravel :

```
php artisan key:generate
```

Configurer la base de données dans `.env`.

Puis lancer les migrations :

```
php artisan migrate
```

Démarrer le serveur local :

```
php artisan serve
```

Application disponible sur :

```
http://localhost:8000
```

---

# Documentation

La documentation technique complète est disponible dans :

```
/docs
```

* architecture.md
* deployment.md
* database.md
* dev-workflow.md
