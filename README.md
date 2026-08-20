# 🐼 Atelier Pandas – Capteurs IoT

## 📌 Contexte

Une entreprise possède plusieurs bâtiments équipés de capteurs IoT collectant température, humidité, pression, consommation énergétique, état du capteur, bâtiment, date et heure de mesure. Cet atelier utilise **Pandas** pour préparer et analyser ces données avant leur transmission à un futur système de Machine Learning de détection d'anomalies.

Atelier réalisé dans le cadre du cours **Python pour ML et IA** – P1 IA, Orange Digital Center (ODC) .

## 🎯 Objectifs

- Manipuler des `Series` et des `DataFrame`
- Explorer, sélectionner et filtrer des données
- Ajouter, renommer et supprimer des colonnes
- Trier et analyser des données par groupe
- Gérer les valeurs manquantes et les doublons
- Calculer des statistiques descriptives
- Exporter des données nettoyées

## 🗂️ Structure du projet

```
atelier_pandas_iot/
├── data/
│   └── mesures_capteurs.csv
├── notebooks/
│   └── atelier_pandas_iot.ipynb
└── exports/
    ├── donnees_nettoyees.csv
    └── donnees_nettoyees.json
```

## 🧩 Contenu de l'atelier

| Partie | Sujet |
|---|---|
| 1 | Series (création, index, valeurs) |
| 2 | DataFrame (création manuelle, import CSV, dimensions) |
| 3 | Exploration (`head`, `tail`, `shape`, `columns`, `info`, `describe`) |
| 4 | Sélection (`loc`, `iloc`, colonnes) |
| 5 | Manipulation des colonnes (ajout, catégorisation, renommage, suppression) |
| 6 | Filtrage (conditions simples et combinées) |
| 7 | Tri (croissant, décroissant, top 10, tri multi-colonnes) |
| 8 | Analyse par groupe (`groupby` : consommation, température, alertes par bâtiment) |
| 9 | Gestion des valeurs manquantes (détection, taux, imputation) |
| 10 | Gestion des doublons (détection, suppression) |
| 11 | Statistiques descriptives (min, max, moyenne, médiane, écart-type, mode) |
| 12 | Exportation (CSV, JSON) |
| 13 | Bonus – fonctionnalité additionnelle pertinente |

## 🧹 Nettoyage des données

- Température et humidité → valeurs manquantes remplacées par la **moyenne**
- Consommation → valeurs manquantes remplacées par la **médiane**
- État (`etat`) → valeurs manquantes remplacées par `"INCONNU"`
- Suppression des doublons

## ▶️ Utilisation

```bash
pip install pandas jupyter
jupyter notebook notebooks/atelier_pandas_iot.ipynb
```

## 📦 Livrable attendu

Dossier `atelier_pandas_iot/` complet, poussé sur un dépôt public GitHub avec commits explicites au fur et à mesure.

## 👤 Auteure

**Rokhaya Coumba Diouf** – parcours IA (P1 IA) Orange Digital Center (ODC)
