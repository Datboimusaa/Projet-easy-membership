📌 EasyMembership (Prototype Web)

EasyMembership est une application web simple destinée aux associations au Sénégal.
Ce prototype permet d’avoir une première version fonctionnelle (MVP) avec :

✔️ Landing page
✔️ Authentification via Firebase
✔️ Dashboard avec rôles (Président / Trésorier / Secrétaire / Membre)
✔️ Ajout de membres
✔️ Ajout d’événements

Ce projet est une version simplifiée du futur système complet EasyMembership.

🚀 Objectifs du MVP

Le but n'est pas de construire toutes les fonctionnalités finales, mais de :

Avoir une interface fonctionnelle (même simple)

Mettre en place l’authentification et gestion des rôles

Créer des pages permettant de gérer des membres et des événements

Déployer le prototype en ligne (Firebase Hosting)

Ce projet servira de démo et base d’amélioration.

🛠️ Technologies utilisées
Technologie	Utilisation
HTML / CSS	Structure et styles
Bootstrap 5	Interface responsive
JavaScript (Vanilla)	Logique côté client
Firebase Authentication	Gestion des comptes utilisateurs
Firebase Firestore	Stockage des données (membres, événements, rôles)
Firebase Hosting	Déploiement
📁 Structure du projet
📦 EasyMembership
│── index.html             → Landing page
│── auth.html              → Login / Register
│── dashboard.html         → Espace utilisateur
│── members.html           → Gestion des membres
│── events.html            → Gestion des événements
│
│── /css
│   └── style.css
│
│── /js
│   ├── firebase-config.js → Connexion Firebase
│   ├── auth.js            → Login / Register / Roles
│   ├── members.js         → CRUD membres
│   └── events.js          → CRUD événements
│
└── README.md

⚙️ Installation (pour les contributeurs)

1️⃣ Cloner le projet

git clone https://github.com/<votre-repo>.git
cd EasyMembership


2️⃣ Installer Firebase CLI (si vous voulez déployer)

npm install -g firebase-tools


3️⃣ Créer un projet Firebase depuis la console Firebase

👉 https://console.firebase.google.com/

4️⃣ Copier les clés Firebase dans firebase-config.js

const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};


5️⃣ Tester localement

Ouvrir vos fichiers dans un navigateur ou utiliser Live Server.

🧪 Fonctions déjà prévues
Fonction	Statut
Landing Page	🟢 OK
Authentification Firebase	🟢 OK
Gestion des rôles	🟡 Basique
Ajouter des membres	🟡 En cours
Ajouter des événements	🟡 En cours
Déploiement Firebase	🟢 OK
🙋‍♂️ Règles pour contribuer

Ne pas modifier firebase-config.js (seulement votre copie locale)

Toujours créer une branche avant modification :

git checkout -b feature-nomFonction


Commit propre et clair :

feat: ajout formulaire membre
fix: bug authentification
style: amélioration mise en page dashboard


Faire une Pull Request → validation avant merge