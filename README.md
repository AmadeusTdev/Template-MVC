Repository destiné à être une template pour pouvoir être réutilisé plus tard pour d'autres projets

### Statut du projet & Qualité
![Last Commit](https://img.shields.io/github/last-commit/QuiEstCe-IUT/BUT-R3.01-SAE?style=flat)

### Technologie
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Repo Size](https://img.shields.io/github/repo-size/QuiEstCe-IUT/BUT-R3.01-SAE?style=flat-square&logo=github&logoColor=white)

## Architecture

```text
.
├── config
│   ├── database.example.php # Modèle à copier en config/database.php (non versionné)
│   └── database.php         # Identifiants réels, IGNORÉ par Git
├── database
│   └── dump.sql
├── core
│   ├── includes             # Autoloader et includes PHP internes
│   ├── utils                # Fonctions utilitaires PHP
│   └── model.php            # Classe Model abstraite : connexion PDO/PostgreSQL partagée
├── public                  # Unique répertoire exposé sur le Web (document root)
│   ├── assets
│   ├── favicon.ico
│   └── index.php            # Routeur central
├── src
│   ├── controllers
│   ├── models
│   └── views
├── .gitignore
└── README.md
```

> `vendor/`, `config/database.php` et `coverage/` ne sont pas versionnés

## Execution

php -S localhost:8000 -t public

Le site est alors accessible sur `http://localhost:8000`.
