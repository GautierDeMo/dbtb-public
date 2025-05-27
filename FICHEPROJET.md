# 🎯 DBTB – Team Builder eXperience

## 🧠 Objectifs du projet
Développer un outil performant et modulaire permettant aux utilisateurs de filtrer, construire, organiser et sauvegarder des équipes personnalisées dans un contexte de jeu mobile.  
L’application vise à offrir une expérience fluide, avec une interface claire, un moteur de recherche avancé, ainsi qu’un système de sauvegarde et de partage.  
Une évolution future pourrait en faire une plateforme communautaire.

## 🚧 Statut du projet
Projet personnel en cours de développement.  
✔️ Premières entités critiques intégrées et testées  
🔜 Prochaine étape : logique de sélection des équipes & interface utilisateur

## 🛠️ Fonctionnalités principales
- 🔎 Moteur de recherche multi-filtres
- 🧱 Construction d’équipes
- 💾 Sauvegarde personnalisée
- 🔗 Partage d’équipes
- 📊 Consultation des détails sur les cartes (leader skills, passives, etc.)

## ⚙️ Stack et outils techniques
- 🐘 Symfony (back-end)
- 🔄 Doctrine ORM
- 🐳 Docker (environnement de dev)
- 🗃️ SQLite
- 💡 PHPStorm (connexion DB & génération DDL)
- 👥 Pair programming ponctuel

### 🔧 Outils open source utilisés

Nous tenons à mentionner deux outils qui ont facilité notre travail :

- [`doctrine-helper`](https://github.com/siburuxue/doctrine-helper) :  
  Un outil CLI qui nous a permis de générer efficacement des entités Doctrine à partir d’une base SQLite.  
  Un vrai gain de temps dans la phase d’intégration des données.

- [`zsh-in-docker`](https://github.com/deluan/zsh-in-docker) :  
  Une image Docker pratique pour intégrer zsh directement dans nos conteneurs Symfony.  
  Cela améliore nettement le confort de développement au quotidien.


## 🧩 Démarche technique
### 🐳 Dockerisation
Utilisation d’une image Symfony prête à l’emploi via `docker compose`, pour un environnement isolé et reproductible.

### 🔁 Reverse engineering
Import d’une base SQLite du jeu, renommage structuré, ajout d’index, puis génération d’entités via CLI personnalisée (`doctrine-helper:mapping:import`).

### 🧼 Méthodologie rigoureuse
Chaque entité suit un process reproductible :
- Suppression des anciennes entités
- Création d’une table de test
- Génération Doctrine via CLI
- Refactorisation manuelle
- Réinitialisation complète entre chaque étape

### 🧠 Bonnes pratiques
- Commits clairs et structurés
- Nettoyage automatique via PHPStorm
- Documentation des décisions techniques

## 🧑‍💻 Compétences mobilisées & développées
- Doctrine & Symfony : génération avancée, relations, CRUD
- Reverse engineering : compréhension d’une base externe
- Autonomie, rigueur, organisation
- Git & bonnes pratiques
- Documentation technique claire

## 👥 Contributeurs
Projet développé en duo par [Gautier] et [Matthias], deux frères passionnés à la fois par le jeu mobile et le développement web.

---
