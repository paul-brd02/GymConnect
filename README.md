# GymConnect

## Description

GymConnect est une application tout en un dédié à la musculation. Cette application permet d’aider les débutants. Notre but est de rentre accessible à tous/toutes, les bases de la musculation, à savoir comment faire les exercices, comment ne pas se blesser, la difficulté de l’exercice et l’efficacité des exercices. 
De plus, GymConnect possède un espace communautaire, qui permet à celles et ceux qui le souhaite, de partager leurs exercices favoris. 
Nos équipes s’engagent à vérifier les exercices et à les notés sur 5, en prenant en compte l’explication ,l’efficacité et la difficulté, avant de les publier sur l’application.  

## Table des matières

- [Prérequis](#prérequis)
- [Installation](#installation)
- [Configuration](#configuration)
- [Utilisation](#utilisation)
- [Equipe](#equipe)

## Prérequis

Assurez-vous d'avoir installé les éléments suivants sur votre machine :

- Python (version 3.7 ou supérieure)
- Node.js et npm (ou yarn)
- PostgreSQL
- `pip` (le gestionnaire de packages Python)
- `virtualenv` (facultatif mais recommandé)

## Installation

### Backend (Django)

1. Clonez le dépôt :
    ```bash
    git clone https://github.com/paul-brd02/GymConnect.git
    cd GymConnect/back
    ```

2. Créez et activez un environnement virtuel :
    ```bash
    python -m venv venv
    # Sur Windows
    venv\Scripts\activate
    # Sur macOS/Linux
    source venv/bin/activate
    ```

3. Installez les dépendances :
    ```bash
    pip install -r requirements.txt
    ```

4. Configurez la base de données dans `GymConnect/settings.py` :
    ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'nom_de_la_base_de_donnees',
            'USER': 'votre_utilisateur',
            'PASSWORD': 'votre_mot_de_passe',
            'HOST': 'localhost',
            'PORT': '5432',
        }
    }
    ```

5. Appliquez les migrations :
    ```bash
    python manage.py migrate
    ```

6. Démarrez le serveur de développement :
    ```bash
    python manage.py runserver
    ```

### Frontend (ReactJS)

1. Naviguez dans le répertoire frontend :
    ```bash
    cd ../front
    ```

2. Installez les dépendances :
    ```bash
    npm install
    ```

3. Démarrez le serveur de développement :
    ```bash
    npm start
    ```

## Configuration

### Backend

- Les fichiers de configuration de Django se trouvent dans le répertoire `back/myproject/settings.py`.
- Assurez-vous de configurer correctement votre base de données PostgreSQL.

### Frontend

- Les configurations de Tailwind CSS se trouvent dans `front/tailwind.config.js`.
- Les fichiers CSS de Tailwind sont importés dans `front/src/index.css`.

## Utilisation

### Backend

L'API backend est accessible à l'adresse `http://127.0.0.1:8000/GymConnect/`.

### Frontend

L'application frontend est accessible à l'adresse `http://localhost:3000/`.

## Equipe
- Paul BARDOU
- Rémi GERONCE
- Mathis TAJAN
- Christal PELOFI