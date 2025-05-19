# 🚀 Installation du projet Symfony

Ce projet Symfony a été développé pour [votre usage ici]. Ce guide explique comment installer et lancer le projet en local.

---

## 📦 Prérequis

Assurez-vous d'avoir les outils suivants installés :
- PHP >= 8.1
- Composer
- Symfony CLI
- MySQL / MariaDB ou PostgreSQL
- Node.js & Yarn (si assets frontend)
- Docker (optionnel mais recommandé)

---

## 🔧 Installation

### 1. Cloner le dépôt
```bash
git clone https://github.com/votre-repo/mon-projet-symfony.git
cd mon-projet-symfony
```

### 2. Installer les dépendances
```bash
composer install
```

### 3. Configurer la base de données
Créez un fichier `.env.local` à la racine du projet et configurez votre connexion à la base de données :
```
DATABASE_URL="mysql://utilisateur:mot_de_passe@127.0.0.1:3306/nom_base_de_donnees"
```

### 4. Créer la base de données
```bash
php bin/console doctrine:database:create
```

### 5. Exécuter les migrations
```bash
php bin/console doctrine:migrations:migrate
```

### 6. Charger les fixtures (données de test)
```bash
php bin/console doctrine:fixtures:load
```

### 7. Installer les dépendances frontend (si nécessaire)
```bash
yarn install
yarn build
```

---

## 🚀 Lancement du serveur

### Avec Symfony CLI
```bash
symfony serve
```
ou avec l'option watch pour le rechargement automatique :
```bash
symfony server:start --watch
```

### Avec PHP built-in server
```bash
php -S localhost:8000 -t public/
```

---

## 🧪 Tests

Pour exécuter les tests :
```bash
php bin/phpunit
```

---

## 📚 Documentation

Pour plus d'informations, consultez la [documentation de Symfony](https://symfony.com/doc/current/index.html).