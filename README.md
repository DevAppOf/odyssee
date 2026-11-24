# Odyssée — Explorateur de pays

## 1. Présentation du projet

**Odyssée** est une application web développée avec React qui permet aux utilisateurs d'explorer les pays du monde, de consulter leurs informations et de découvrir les différentes régions et continents.

L'application utilise l'API **REST Countries** pour récupérer les données des pays.

## 2. Cahier des charges

### Objectif du projet

Développer une application web interactive permettant de rechercher, filtrer et consulter les informations des pays du monde.

## 3. Groupes et sujet

### Groupe

- Kahide BOHUI
- Aliou DIARRA
- Serkan YIGIT

### Sujet retenu

**Explorateur de pays**

### API utilisée

[restcountries](https://restcountries.com/v3.1)

Cette API permet de récupérer des informations sur les pays du monde : nom, capitale, etc.

### Fonctionnalités envisagées

- Recherche d'un pays par son nom.
- Filtrage des pays par continent.
- Consultation de la fiche détaillée d'un pays.
- Ajout de pays aux favoris.
- Gestion des pays visités.

## 4. Maquette des pages

RAS

## 5. Arborescence du projet

```text
odyssee/
│
├── public/
│
├── src/
│   │
│   ├── assets/
│   │   └── images/
│   │
│   ├── components/
│   │   ├── layout/
│   │   │   ├── Navigation.jsx
│   │   │   └── Footer.jsx
│   │   │
│   │   ├── home/
│   │   │   ├── Hero.jsx
│   │   │   ├── SearchBar.jsx
│   │   │   ├── ContinentFilter.jsx
│   │   │   ├── CountryGrid.jsx
│   │   │   ├── CountryCard.jsx
│   │   │   ├── CountryModal.jsx
│   │   │   ├── FavoriteButton.jsx
│   │   │   └── QuoteSection.jsx
│   │   │
│   │   └── auth/
│   │       ├── LoginForm.jsx
│   │       ├── SignupForm.jsx
│   │       └── InputField.jsx
│   │
│   ├── data/
│   │   └── countries.js
│   │
│   ├── hooks/
│   │   ├── useFetch.js
│   │   ├── useCountryFilter.js
│   │   └── useFavorites.js
│   │
│   ├── pages/
│   │   ├── HomePage.jsx
│   │   ├── AuthPage.jsx
│   │   ├── CountryDetailPage.jsx
│   │   ├── VisitedPage.jsx
│   │   └── NotFoundPage.jsx
│   │
│   ├── styles/
│   │   ├── variables.css
│   │   └── global.css
│   │
│   ├── App.jsx
│   └── main.jsx
│
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

## 6. Rôle des principaux dossiers et fichiers

| Dossier / Fichier    | Responsabilité                                                                                          |
| -------------------- | ------------------------------------------------------------------------------------------------------- |
| `public/`            | Contient les ressources statiques accessibles directement, sans traitement par Vite.                    |
| `src/`               | Contient le code source principal de l'application.                                                     |
| `assets/`            | Stocke les ressources visuelles du projet (images, illustrations, etc.).                                |
| `components/`        | Regroupe les composants réutilisables de l'interface.                                                   |
| `components/layout/` | Contient les éléments communs aux différentes pages : navigation et pied de page.                       |
| `components/home/`   | Regroupe les composants propres à la page d'accueil : recherche, filtres, cartes et affichage des pays. |
| `components/auth/`   | Contient les composants des formulaires de connexion et d'inscription.                                  |
| `data/`              | Centralise les données relatives aux pays lorsque des données locales sont nécessaires.                 |
| `hooks/`             | Regroupe la logique React réutilisable : récupération des données, filtres et favoris.                  |
| `pages/`             | Contient les différentes pages accessibles par les routes de l'application.                             |
| `styles/`            | Centralise les feuilles de style CSS et les variables graphiques.                                       |

### Rôle des principaux fichiers

| Fichier                 | Responsabilité                                                                               |
| ----------------------- | -------------------------------------------------------------------------------------------- |
| `App.jsx`               | Configure les routes et organise les pages de l'application.                                 |
| `main.jsx`              | Point d'entrée de l'application React.                                                       |
| `useFetch.js`           | Gère la récupération des données depuis l'API ainsi que les états de chargement et d'erreur. |
| `useCountryFilter.js`   | Gère la recherche et le filtrage des pays.                                                   |
| `useFavorites.js`       | Gère les pays favoris et leur conservation après rechargement.                               |
| `HomePage.jsx`          | Affiche la page d'accueil et la liste des pays.                                              |
| `CountryDetailPage.jsx` | Affiche les informations détaillées d'un pays sélectionné.                                   |
| `VisitedPage.jsx`       | Affiche les pays marqués comme visités.                                                      |
| `NotFoundPage.jsx`      | Affiche une page d'erreur lorsque l'utilisateur accède à une route inexistante.              |
| `Navigation.jsx`        | Affiche le menu de navigation entre les pages.                                               |
| `Footer.jsx`            | Affiche le pied de page de l'application.                                                    |

## 7. Technologies utilisées

- **React** : création de l'interface utilisateur.
- **Vite** : environnement de développement et outil de construction.
- **React Router** : gestion de la navigation entre les pages.
- **JavaScript** : développement des fonctionnalités.
- **CSS** : mise en forme et design de l'application.
- **REST Countries API** : récupération des informations sur les pays.
- **Git et GitHub** : gestion des versions et travail collaboratif.
- **Vercel ou Netlify** : hébergement de l'application.

## 8. Installation et lancement du projet

### Prérequis

- Node.js
- npm
- Git

### Installation

Cloner le dépôt :

```bash
git clone URL_DU_DEPOT
```

Accéder au dossier du projet :

```bash
cd odyssee
```

Installer les dépendances :

```bash
npm install
```

Lancer le serveur de développement :

```bash
npm run dev
```

## 9. Déploiement

**Plateforme de déploiement :** RAS

**Lien de la version en ligne :** RAS
