# Application de Gestion des Affectations des Enseignements

## Contexte
Ce projet est une application web développée dans le cadre du module « Web 1 : Technologies du Web et PHP5 » (A.U. 2024/2025, Filière GI1, Prof : E. W. DADI). Elle vise à optimiser et automatiser l'affectation des unités d'enseignement (UE) aux enseignants au sein des départements académiques, tout en assurant une répartition équilibrée et transparente des charges horaires.

## Objectifs
- Centraliser la gestion des unités d'enseignement et des enseignants par département.
- Simplifier l'expression des souhaits des enseignants pour l'année universitaire suivante.
- Assurer une répartition équilibrée des charges horaires.
- Permettre aux responsables de gérer et valider l'affectation des enseignements.
- Générer des rapports détaillés pour le suivi et l'analyse.
- Assurer la traçabilité des décisions et l'historique des affectations.

## Fonctionnalités principales
- Authentification sécurisée multi-rôles (admin, chef de département, coordonnateur, enseignant, vacataire)
- Gestion centralisée des UE, enseignants, filières et départements
- Expression des vœux d'enseignement par les professeurs
- Affectation et validation des enseignements par les responsables
- Calcul et suivi automatique des charges horaires
- Import/export de données (Excel)
- Génération de rapports et historique des affectations
- Gestion des notes (upload, consultation)

## Rôles et permissions
- **Administrateur** : Gestion des comptes, création des professeurs, affectation des responsabilités
- **Chef de département** : Gestion des modules et professeurs du département, affectation et validation des UE, reporting, gestion des UE vacantes
- **Coordonnateur de filière** : Gestion des modules de la filière, affectation des vacataires, gestion des emplois du temps, import/export
- **Enseignant** : Sélection des UE, suivi de la charge horaire, upload des notes, consultation de l'historique
- **Vacataire** : Consultation des UE affectées, gestion des notes

## Installation et configuration
1. **Prérequis**
   - PHP >= 7.4
   - Serveur web (Apache, Nginx, etc.)
   - MySQL/MariaDB
   - [Composer](https://getcomposer.org/) pour la gestion des dépendances

2. **Cloner le projet**
   ```bash
   git clone <repo-url>
   cd <nom-du-dossier>
   ```

3. **Installer les dépendances PHP**
   ```bash
   composer install
   ```

4. **Configurer la base de données**
   - Créez une base de données MySQL/MariaDB
   - Importez le fichier `database.sql`
   - Modifiez les paramètres de connexion dans `config/database.php` si nécessaire

5. **Configurer les droits d'écriture**
   - Assurez-vous que le dossier `uploads/` est accessible en écriture par le serveur web

## Utilisation
- Accédez à la page de connexion (`login.php`)
- Connectez-vous avec un compte correspondant à votre rôle (admin, chef de département, etc.)
- Naviguez selon les permissions de votre rôle pour gérer les affectations, modules, notes, etc.

## Dépendances
- [PHPMailer](https://github.com/PHPMailer/PHPMailer) (pour l'envoi d'e-mails)
- Bootstrap, FontAwesome (CDN, pour le style)

## Auteurs
Aya BOUIBAUAN
Safae BIFKIOUN
Rachida Amourak


## Licence
Ce projet est à usage académique dans le cadre du module Web1. 