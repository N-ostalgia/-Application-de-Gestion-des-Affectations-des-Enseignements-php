
# 🎓 Application de Gestion des Affectations des Enseignements

![PHP Version](https://img.shields.io/badge/PHP-%3E%3D7.4-blue)
![License](https://img.shields.io/badge/License-Academic--Use-lightgrey)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

> Projet Web réalisé dans le cadre du module **« Web 1 : Technologies du Web et PHP5 »**  
> _Année Universitaire 2024/2025 — Filière GI1 — 

---

## 🧭 Sommaire

- [Contexte](#-contexte)
- [Objectifs](#-objectifs)
- [Fonctionnalités principales](#-fonctionnalités-principales)
- [Rôles et permissions](#-rôles-et-permissions)
- [Installation et configuration](#-installation-et-configuration)
- [Utilisation](#-utilisation)
- [Dépendances](#-dépendances)
- [Auteurs](#-auteurs)
- [Licence](#-licence)

---

## 📌 Contexte

Cette application web a été conçue pour **optimiser** et **automatiser** le processus d’affectation des unités d’enseignement (UE) aux enseignants dans les départements académiques, tout en garantissant une **répartition équilibrée** et **transparente** des charges horaires.

---

## 🎯 Objectifs

- 🗂️ Centraliser la gestion des UE, enseignants et départements
- 💬 Simplifier l’expression des souhaits des enseignants
- ⚖️ Équilibrer les charges horaires automatiquement
- 🧑‍💼 Permettre la gestion/validation des affectations par les responsables
- 📄 Générer des rapports détaillés pour le suivi
- 🕓 Assurer la traçabilité et l’historique des affectations

---

## ⚙️ Fonctionnalités principales

- 🔐 Authentification multi-rôles sécurisée (Admin, Chef de Département, Coordonnateur, Enseignant, Vacataire)
- 🧑‍🏫 Gestion centralisée des enseignants, modules, filières, départements
- 🎯 Saisie des vœux d’enseignement
- ✅ Validation des affectations
- 🧮 Suivi automatique des charges horaires
- 📤📥 Import/Export de données (Excel)
- 🧾 Génération de rapports
- 📝 Gestion et consultation des notes

---

## 👥 Rôles et permissions

| Rôle                 | Actions principales |
|----------------------|---------------------|
| 🛠️ **Administrateur**        | Création de comptes, gestion des rôles |
| 🧑‍🏫 **Chef de département** | Affectation/validation des UE, gestion modules et professeurs, reporting |
| 📚 **Coordonnateur**        | Gestion des modules de filière, vacataires, emplois du temps |
| 👨‍🎓 **Enseignant**           | Choix des UE, suivi de charge horaire, gestion des notes |
| 🧑‍💻 **Vacataire**            | Consultation des affectations et gestion des notes |

---

## 🛠️ Installation et configuration

### 1. Prérequis

- PHP ≥ 7.4  
- Serveur web (Apache ou Nginx)  
- MySQL ou MariaDB  
- [Composer](https://getcomposer.org/) installé

### 2. Cloner le projet

```bash
git clone https://github.com/N-ostalgia/-Application-de-Gestion-des-Affectations-des-Enseignements-php.git
cd Application-de-Gestion-des-Affectations-des-Enseignements-php
```

### 3. Installer les dépendances PHP

```bash
composer install
```

### 4. Configurer la base de données

- Créez une base de données MySQL/MariaDB
- Importez le fichier `database.sql`
- Mettez à jour les identifiants dans `config/database.php` :

```php
define('DB_HOST', 'localhost');
define('DB_USER', 'votre_utilisateur');
define('DB_PASS', 'votre_mot_de_passe');
define('DB_NAME', 'nom_de_la_base');
```

### 5. Configurer les droits d'écriture

Assurez-vous que les dossiers suivants sont accessibles en écriture :

```bash
chmod -R 755 uploads/
```

---

## 🚀 Utilisation

1. Ouvrez votre navigateur et accédez à `http://localhost/login.php`
2. Connectez-vous avec un compte correspondant à votre rôle (admin, enseignant, etc.)
3. Naviguez dans l’interface pour gérer les UE, affectations, emplois du temps ou notes selon votre rôle.

---

## 📦 Dépendances

- [PHPMailer](https://github.com/PHPMailer/PHPMailer) — pour l’envoi d’e-mails
- [Bootstrap](https://getbootstrap.com/) — framework CSS responsive
- [FontAwesome](https://fontawesome.com/) — bibliothèque d’icônes
- [Composer](https://getcomposer.org/) — gestionnaire de dépendances PHP

---

## 👩‍💻 Auteurs

- Aya **BOUIBAUAN**  
- Safae **BIFKIOUN**  
- Rachida **AMOURAK**

---

## 📝 Licence

Ce projet est destiné uniquement à un usage **académique**, réalisé dans le cadre du module **Web 1 : Technologies du Web et PHP5** — Filière GI1, 2024/2025.
