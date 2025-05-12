##PGR301 Exam

Add environment variables  before doing anything else, then run the application.

##Environment variables

Set your own environment variables.  

* DOCKER_USERNAME
* DOCKER_PASSWORD
* GRAFANA_AUTH
* GRAFANA_URL

Set up environment variables ex.: "export DOCKER_USERNAME=your_username"

##Content
- Repository with both infrastructure and application
- Embedded H2 database, accessible through localhost:8080/h2
- Docker builds a container image of the application
- Travis builds a new image for every commit

# Sample App

## Description de l'application

Cette application est une **web app simple** développée avec [technologie choisie] (ex. Node.js, Flask, Spring Boot). Elle permet de [expliquer brièvement ce que fait l'application, par exemple : gérer des utilisateurs, afficher des produits, etc.].

## Configuration DevOps (Pipeline CI/CD)

### 1. GitLab CI/CD

Le projet utilise **GitLab CI/CD** pour automatiser les processus suivants :

- **Build de l'application** : À chaque push sur la branche `feature/devops-pipeline`, un pipeline CI est déclenché pour compiler et tester l'application.
- **Tests automatisés** : Des tests unitaires et d'intégration sont exécutés pendant le processus de build pour assurer la qualité du code.
- **Dockerisation** : L'application est conteneurisée dans une image Docker et cette image est ensuite poussée vers un registre GitLab.
- **Déploiement sur Kubernetes** : Une fois l'image Docker disponible, elle est déployée sur un cluster Kubernetes pour être mise en production.

### 2. Jenkins

Le déploiement est orchestré par **Jenkins** qui récupère le code source depuis GitLab, construit l'image Docker, puis déploie l'application sur un cluster Kubernetes en utilisant les fichiers YAML de configuration.

### 3. Kubernetes

Kubernetes est utilisé pour l'orchestration des conteneurs, garantissant la gestion, la mise à l'échelle, et la haute disponibilité de l'application en production.

---

### 🔹 Étape 3 : Sauvegarder les modifications

Après avoir modifié le `README.md`, enregistre et ferme l'éditeur (par exemple, avec `CTRL+O`, `ENTER`, puis `CTRL+X` dans `nano`).

---

### 🔹 Étape 4 : Valider et pousser les modifications

1. Ajoute les modifications au suivi de Git :

```bash
git add README.md
