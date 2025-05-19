# 🚀 Installation du projet Symfony

Ce projet Symfony a été développé pour [votre usage ici]. Ce guide explique comment installer et lancer le projet en local.

---

## 📦 Prérequis

Assurez-vous d’avoir les outils suivants installés :

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

```bash
composer install

```bash
php bin/console doctrine:migrations:migrate

```bash
php bin/console doctrine:fixtures:load

```bash
symfony server:watch


