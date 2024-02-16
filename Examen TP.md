### Examen Technique de MLOps sur les Critiques de Films - Durée : 2 Heures

#### Objectif de l'Examen
Cet examen vise à évaluer vos compétences en MLOps en vous faisant travailler sur un projet de classification des critiques de films. Vous utiliserez GitLab pour l'automatisation CI/CD et Docker pour la conteneurisation.

#### Contexte
Vous êtes un Data Scientist dans une entreprise de streaming vidéo en ligne. On vous demande de mettre en place un système pour classer automatiquement les critiques de films en deux catégories : positives (1) et négatives (0), en utilisant les pratiques MLOps.

#### Instructions
Vous disposerez de 2 heures pour compléter cet examen qui se divise en quatre parties principales.

#### Partie 1 : Préparation du Dataset (30 minutes)
1. Téléchargez le fichier `reviews_unique.csv` contenant les critiques de films et leurs labels associés.
2. Explorez rapidement le dataset pour comprendre sa structure et effectuez un prétraitement simple si nécessaire (par exemple, suppression des doublons).

#### Partie 2 : Entraînement d'un Modèle de Machine Learning (30 minutes)
1. Utilisez Python pour développer un script (`train_model.py`) qui entraîne un modèle de classification (par exemple, Logistic Regression) sur le dataset.
2. Votre script doit inclure une phase de validation pour évaluer la performance du modèle (par exemple, précision, rappel).
3. Sauvegardez le modèle entraîné pour une utilisation ultérieure.

#### Partie 3 : Conteneurisation avec Docker (30 minutes)
1. Créez une API Flask simple avec un endpoint `/predict` qui prend une critique de film en entrée et retourne la prédiction du modèle (positif/négatif).
2. Conteneurisez votre application Flask et le modèle entraîné en utilisant Docker. Fournissez le `Dockerfile` correspondant.

#### Partie 4 : Automatisation CI/CD avec GitLab (30 minutes)
1. Configurez un pipeline CI/CD dans GitLab à l'aide d'un fichier `.gitlab-ci.yml`. Le pipeline doit effectuer les tâches suivantes :
   - Construction de l'image Docker de votre application Flask.
   - Exécution de tests unitaires simples pour vérifier la fonctionnalité de l'API.
   - (Optionnel) Déploiement de l'image Docker sur un registre d'images Docker.

#### Critères d'Évaluation
- Qualité et clarté du code Python pour l'entraînement du modèle.
- Efficacité et précision du modèle de classification.
- Complétude et fonctionnalité du `Dockerfile`.
- Configuration correcte et fonctionnement du pipeline CI/CD dans `.gitlab-ci.yml`.

#### Livrables
- Script Python `train_model.py` pour l'entraînement et l'évaluation du modèle.
- `Dockerfile` pour conteneuriser votre application Flask.
- Fichier `.gitlab-ci.yml` pour la configuration de votre pipeline CI/CD.

#### Remarques
- Assurez-vous de commenter votre code pour expliquer votre logique.
- Testez votre API Flask localement avant de la conteneuriser pour vous assurer qu'elle fonctionne comme prévu.
- Veillez à ce que votre pipeline CI/CD soit optimisé et ne contienne pas d'étapes inutiles.

Bonne chance !
