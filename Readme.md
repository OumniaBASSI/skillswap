#  SkillSwap – README

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

## ✨ Fonctionnalités

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

