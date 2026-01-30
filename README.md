# 📊 Analyse des courses Yellow Taxi – EDA & Statistiques

## 📌 Contexte du projet

Dans un contexte de **données massives de mobilité urbaine**, les Data Analysts sont souvent confrontés à un choix méthodologique clé :

> **Faut-il analyser un échantillon de données et inférer la population, ou traiter l’ensemble des données via des technologies Big Data ?**

Ce projet s’inscrit dans cette problématique et vise à comparer **deux approches analytiques** appliquées aux données des courses de taxis à New York entre **2022 et 2024** :

- 🔹 **Approche de statistiques inférentielles** basée sur un échantillon de **1 %**
- 🔹 **Approche Big Data** exploitant **100 % des données** avec **Apache Spark**

🎯 **Objectif global** :  
Comprendre les **avantages, limites et compromis** de chaque approche dans un contexte métier réel.

---

## 🎯 Objectifs

- Explorer la **structure** et le **contenu** des données
- Vérifier la **qualité des données** :
  - valeurs manquantes
  - doublons
  - outliers
- Analyser les **distributions** des variables clés :
  - distance
  - prix
  - tips
  - durée des courses
- Réaliser des **analyses statistiques** :
  - moyennes
  - proportions
  - intervalles de confiance
- Comparer les résultats :
  - avec et sans outliers
  - échantillon vs population
- Appliquer la **même logique d’analyse** sur le Big Data

---

## 🧪 Méthodologie suivie

Le projet suit un **workflow Data Analyst professionnel**, commun aux deux approches.

### 1️⃣ Prise en main des données & EDA
- Compréhension des variables
- Analyse des distributions
- Étude des valeurs manquantes
- Vérification de la cohérence des données

### 2️⃣ Approche statistiques inférentielles (Échantillon)
- Calcul des indicateurs clés
- Intervalles de confiance
- Analyse de la représentativité
- Détection et analyse des outliers

### 3️⃣ Approche Big Data (Population complète)
- Chargement des données avec **Spark**
- Agrégations à grande échelle
- Calcul des **valeurs exactes de la population**

### 4️⃣ Comparaison des résultats
- Échantillon vs population
- Biais potentiels
- Impact des outliers
- Pertinence métier des résultats

---

## 📁 Structure du projet

```text
├── notebook_echantillon.ipynb
│   └── Analyse complète sur l’échantillon (EDA + statistiques)
│
├── notebook_big_data.ipynb
│   └── Analyse Big Data sur l’ensemble des courses Yellow Taxi
│
├── echantillon/
│   └── Fichier CSV de l’échantillon (1 %)
│
├── yellow_taxi/
│   └── 36 fichiers du jeu de données complet (Big Data)
