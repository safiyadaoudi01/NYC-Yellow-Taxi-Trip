📊 Analyse des courses Yellow Taxi – EDA & Statistiques
📌 Contexte du projet

Dans un contexte de données massives de mobilité urbaine, les Data Analysts sont souvent confrontés à un choix méthodologique clé :

Faut-il analyser un échantillon de données et inférer la population, ou traiter l’ensemble des données via des technologies Big Data ?

Ce projet s’inscrit dans cette problématique et vise à comparer deux approches analytiques appliquées aux données des courses de taxis à New York entre 2022 et 2024 :

Une approche statistiques inférentielles basée sur un échantillon de 1 %

Une approche Big Data exploitant 100 % des données avec Apache Spark

L’objectif est de comprendre les avantages, limites et compromis de chaque approche dans un contexte métier réel.

🎯 Objectifs

Explorer la structure et le contenu des données

Vérifier la qualité des données (valeurs manquantes, doublons, outliers)

Analyser les distributions des variables clés (distance, prix, tips, etc.)

Réaliser des analyses statistiques (moyennes, proportions, intervalles de confiance)

Comparer les résultats avec et sans outliers

Appliquer la même logique d’analyse sur le Big Data


🧪 Méthodologie suivie

Le projet suit un workflow Data Analyst professionnel, commun aux deux approches :

Prise en main des données & EDA

Compréhension des variables

Analyse des distributions

Valeurs manquantes

Cohérence des données

Approche statistiques inférentielles (échantillon)

Calcul des indicateurs clés

Intervalles de confiance

Analyse de représentativité

Détection et analyse des outliers

Approche Big Data (population complète)

Chargement des données avec Spark

Agrégations à grande échelle

Calcul des valeurs exactes de la population

Comparaison des résultats

Échantillon vs population

Biais potentiels

Impact des outliers

Pertinence métier

📁 Structure du projet

notebook_echantillon.ipynb
→ Analyse complète sur l’échantillon (EDA + statistiques)

notebook_big_data.ipynb
→ Analyse sur l’ensemble des fichiers Yellow Taxi (Big Data)

echantillon/
→ Contient le fichier CSV de l’échantillon

yellow_taxi/
→ Contient 36 fichiers du jeu de données complet (Big Data)

Tous les fichiers de données sont disponibles sur ce dépôt GitHub afin de permettre la reproduction complète de l’analyse.

⚠️ Remarque importante sur les chemins des fichiers
🔹 Notebook Échantillon

Dans le notebook de l’échantillon, le chemin utilisé est :

'/Volumes/workspace/trips/echantillon/yellowtaxisample1pct_hybrid_stratified.csv'


➡️ Action requise pour le visiteur :
Après avoir cloné ou téléchargé le dépôt GitHub, vous devez modifier ce chemin afin qu’il corresponde à l’emplacement local du fichier sur votre machine.

🔹 Notebook Big Data

Dans le notebook Big Data, les fichiers sont chargés via le dossier suivant :

folder = "/Volumes/workspace/trips/yellow_taxi"
files = dbutils.fs.ls(folder)


➡️ Le dossier yellow_taxi contient 36 fichiers analysés dans le notebook.
➡️ Ces fichiers sont également uploadés sur GitHub.
➡️ Le visiteur doit adapter le chemin folder selon son environnement local ou cloud (Databricks, local, etc.).

✅ Reproductibilité

Tous les notebooks sont exécutables

Les données nécessaires sont fournies dans le dépôt

Seule la modification des chemins de fichiers est requise

🛠️ Technologies utilisées

Python

Pandas, NumPy

Matplotlib / Seaborn

SciPy

Environnement Databricks (pour le Big Data)
