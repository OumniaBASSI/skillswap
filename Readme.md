# SkillSwap – README

## Table des matières

1. [Présentation du projet](#présentation-du-projet)
2. [Problèmes à résoudre](#problèmes-à-résoudre)
    - [Problèmes rencontrés](#problèmes-rencontrés)
    - [Besoins exprimés](#besoins-exprimés)
3. [Utilisateurs cibles et rôles](#utilisateurs-cibles-et-rôles)
    - [Lien avec les technologies](#lien-avec-les-technologies)
4. [Fonctionnalités](#fonctionnalités)
    - [Utilisateur simple](#utilisateur-simple)
    - [Administrateur](#administrateur)
5. [User Stories](#user-stories)
6. [Priorisation des fonctionnalités](#priorisation-des-fonctionnalités)
7. [Planification du projet](#planification-du-projet)
   - [Liste des tâches à réaliser](#liste-des-tâches-à-réaliser)
   - [Outils nécessaires au développement](#outils-nécessaires-au-développement)
   - [Outils nécessaires à lexploitation](#outils-nécessaires-à-lexploitation)
8. [Contraintes techniques](#contraintes-techniques)
9. [UML](#uml)

## Présentation du projet

**Nom du projet** : SkillSwap  
**Description** : Plateforme web permettant aux utilisateurs d’échanger des compétences entre eux, sans paiement.  
**Objectif principal** : Faciliter le partage de savoir-faire entre particuliers via un système de troc de compétences.

---

## Problèmes à résoudre

### Problèmes rencontrés :
- Difficulté à trouver des cours personnalisés ou abordables.
- Peu de plateformes favorisent l’échange mutuel de compétences sans paiement.

### Besoins exprimés :
- Offrir un espace simple et gratuit pour apprendre et enseigner entre particuliers.
- Permettre aux utilisateurs de proposer des échanges (ex : “je t’aide en anglais, tu m’aides en Photoshop”).

---

##  Utilisateurs cibles et rôles

| Type d'utilisateur | Description | Rôles et permissions |
|--------------------|-------------|-----------------------|
| **Visiteur** | Non inscrit | - Consulter la page d’accueil<br>- Voir des profils publics |
| **Utilisateur inscrit** | Membre de la plateforme | - Gérer son profil<br>- Publier des offres d’échange<br>- Rechercher des partenaires<br>- Envoyer/recevoir des propositions<br>- Utiliser la messagerie<br>- Noter après un échange |
| **Admin** | Gestionnaire de la plateforme | - Gérer les utilisateurs<br>- Modérer les offres<br>- Supprimer le contenu abusif<br>- Superviser les évaluations |

### Lien avec les technologies
- **Laravel** : Middleware `auth`, `role`, Policies
- **React** : Routes protégées selon les rôles

---

## Fonctionnalités

###  Utilisateur simple
- Inscription / Connexion
- Création & gestion de profil
- Publication d’offres d’échange
- Recherche de partenaires par compétence
- Envoi de propositions d’échange
- Messagerie privée
- Évaluation post-échange

### Administrateur
- Gestion des utilisateurs
- Suppression / modification d’offres
- Supervision des évaluations

---

##  User Stories

- En tant que **visiteur**, je veux **voir des profils et m’informer**, afin de **décider si je veux m’inscrire**.
- En tant qu’**utilisateur inscrit**, je veux **publier une offre d’échange**, afin de **trouver un partenaire pour apprendre une nouvelle compétence**.
- En tant qu’**admin**, je veux **gérer les comptes et contenus**, afin de **garantir la qualité de la plateforme**.

---

## Priorisation des fonctionnalités

| Fonctionnalité | Priorité |
|----------------|----------|
| Inscription/Connexion | 🟢 Essentielle |
| Gestion de profil | 🟢 Essentielle |
| Recherche et filtrage | 🟢 Essentielle |
| Envoi de propositions | 🟢 Essentielle |
| Notation/commentaire | 🟡 Secondaire |
| Tableau de bord admin | 🟢 Essentielle |
| Statistiques détaillées | 🟠 Bonus |

---

## Contraintes techniques

- **Frameworks** : Laravel (Backend), React (Frontend)
- **Base de données** : MySQL
- **Hébergement prévu** : Hostinger
- **Responsive** : Compatible PC, tablette et mobile

---




## Planification du Projet 

---

### Liste des tâches à réaliser

#### Conception (4 jours)
- Création des diagrammes UML (cas d'utilisation, classes, séquence)
- Réalisation des maquettes des interfaces clés 
- Définition de l’architecture du projet 

#### Développement Back-End (6 jours)
- Initialisation du projet Laravel + configuration de la base de données
- Implémentation de l’authentification (inscription, connexion, middleware)
- Création des modèles, contrôleurs, routes API (utilisateurs, offres, demandes)
- Gestion des permissions via Policies (rôles : utilisateur, admin)

#### Développement Front-End (6 jours)
- Initialisation du projet React avec Vite
- Création des pages principales : Accueil, Connexion, Tableau de bord, Offres
- Connexion à l’API + affichage conditionnel selon les rôles

#### Tests (2 jours)
- Tests fonctionnels sur les formulaires, les échanges et les connexions
- Vérification des validations côté front et back
- Tests de sécurité 
#### Déploiement (2 jours)
- Préparation de la version de production
- Déploiement du back-end et front-end sur Hostinger
- Tests post-déploiement 

---
###  Outils nécessaires au développement

#### Langages & Frameworks
- **Back-End** : PHP (Laravel)
- **Front-End** : JavaScript (React)
- **Base de données** : MySQL

#### Environnement de développement
- IDE : Visual Studio Code
- Serveur local : XAMPP
- Navigateurs de test : Chrome, Firefox, Edge

#### Versioning & collaboration
- Git (en local)
- GitHub (hébergement distant du code)

#### Design & UI
- StarUML pour les diagrammes
- Figma pour les maquettes
- Tailwind CSS/ Bootstrap pour le style
- FontAwesome / Lucide Icons pour les icônes

---

### Outils nécessaires à l’exploitation

| Besoin                         | Solution prévue                        |
|--------------------------------|----------------------------------------|
| **Hébergement**                | Hostinger                              |
| **Monitoring & logs**          | Laravel Log     |
| **Sauvegarde base de données** | Automatisée via Hostinger              |
| **Sécurité**                   | Certificat SSL/TLS (Hostinger), pare-feu intégré |

---
## UML
- **Use Case Diagram** :
![Diagramme UML](document/UseCaseDiagram.jpg)
- **Class Diagram** :
![Diagramme UML](document/ClassDiagram1.jpg)
