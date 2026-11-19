# FIT YOUR BOOTY

Application web permettant de suivre ses données personnelles  nutritionnelles, sportives, et de santé.

L'application se divise en trois onglets
* Nutrition & Neat : Suivi des calories, macro, poids, steps, dépense énergétique
     répartie en 3 cards :
              - formulaire d'entrée des données
              - graphique zoomable pour le suivi chronologique des métriques
              - tableau récapitulatif des entrées avec possibilité de modification


* Sport  : Suivi des séances de sport cardio / musculation
            - choix des séances / exercices / métriques
            - graphique pour le suivi chronologique des métriques selon plusieurs aggrégations.
             
* Santé  : Suivi de marqueurs biologiques d'analyse sanguine



Le projet est déployé sur un **VPS Linux** et le code est versionné via **GitHub**.

---

# Stack technique

* Laravel
* PHP 8+
* MySQL / MariaDB
* JavaScript
* Chart.js
* Git / GitHub
* VPS Linux (Ubuntu)

---

# Installation locale

Cloner le projet :

```
git clone git@github.com:SebV-code/fit.git
cd fit
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
