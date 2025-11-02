# Scraper ETL Pipeline

Un pipeline ETL complet qui scrape un site web, nettoie et normalise les données, puis les charge dans une base de données PostgreSQL.

## 📋 Vue d'ensemble

Ce projet est structuré en plusieurs sprints pour apprendre progressivement :
- Web Scraping éthique
- Pipeline ETL (Extract, Transform, Load)
- Gestion de base de données avec SQLAlchemy
- Dockerisation et orchestration
- Logs structurés

## 🚀 Installation

### Prérequis

- Python 3.10 ou supérieur
- pip (gestionnaire de paquets Python)
- PostgreSQL (pour les sprints suivants)
- Docker et Docker Compose (pour les sprints suivants)

### Étapes d'installation

1. **Cloner le dépôt** (si applicable)
   ```bash
   git clone <url-du-repo>
   cd scraper
   ```

2. **Créer un environnement virtuel**
   ```bash
   python -m venv venv
   ```

3. **Activer l'environnement virtuel**
   
   Sur Windows :
   ```powershell
   .\venv\Scripts\Activate.ps1
   ```
   
   Sur Linux/Mac :
   ```bash
   source venv/bin/activate
   ```

4. **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   ```

5. **Configurer les variables d'environnement**
   ```bash
   cp .env.example .env
   ```
   
   Puis éditez le fichier `.env` avec vos valeurs de configuration (ne commitez jamais le fichier `.env` !)

## 📁 Structure du projet

```
scraper/
├── src/              # Code source principal
├── config/           # Fichiers de configuration
├── tests/            # Tests unitaires et d'intégration
├── docker/           # Configuration Docker
├── .env.example      # Exemple de variables d'environnement
├── .gitignore        # Fichiers à ignorer par Git
├── requirements.txt  # Dépendances Python
└── README.md         # Ce fichier
```

## 🎯 Sprints

- **Sprint 1** : Setup initial (✅ En cours)
- **Sprint 2** : Web Scraping basique
- **Sprint 3** : Transformation des données
- **Sprint 4** : Modélisation et base de données
- **Sprint 5** : Pipeline ETL et idempotence
- **Sprint 6** : Logging et Docker

Voir `backlog.md` pour plus de détails sur chaque sprint.

## 🔧 Configuration

Les variables d'environnement sont gérées via le fichier `.env`. Copiez `.env.example` vers `.env` et configurez :

- **Base de données** : Connexion PostgreSQL
- **Scraping** : User-agent, délais, timeout
- **Logs** : Niveau et format de logging

## 📚 Technologies utilisées

- `httpx` : Client HTTP asynchrone
- `selectolax` : Parseur HTML rapide
- `pandas` : Manipulation et transformation de données
- `sqlalchemy` : ORM pour PostgreSQL
- `python-dotenv` : Gestion des variables d'environnement

## 📝 Licence

À définir selon vos besoins.

---
