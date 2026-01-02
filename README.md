# Prévision de la Demande Énergétique avec LSTM

Projet de prédiction de consommation électrique pour Smart Grid utilisant les réseaux de neurones LSTM.

## 📋 Contexte

La start-up **EcoVolt** gère un réseau intelligent de distribution d'électricité et souhaite anticiper les pics de charge pour éviter les surcharges du réseau.

**Objectif** : Prédire la consommation électrique de l'heure suivante (t+1) à partir des 24 heures précédentes.

## 🎯 Problème IA

- **Type** : Régression supervisée sur série temporelle
- **Entrée** : Séquence de 24 heures consécutives
- **Sortie** : Consommation électrique à l'heure suivante (MW)

## 📊 Dataset

Le dataset contient des données horaires avec les colonnes suivantes :

- **DateTime** : Date et heure de la mesure
- **Consumption** : Consommation électrique totale (MW) - *variable cible*
- **Variables explicatives** : Production (Nuclear, Wind, Solar, Hydroelectric, Coal, Oil and Gas, Biomass)

## 🛠️ Technologies

- Python
- TensorFlow/Keras
- Pandas, NumPy
- Scikit-learn
- Matplotlib

## 📂 Structure du Projet

- `dataset.csv` : Données de consommation et production énergétique
- `notebook.ipynb` : Notebook Google Colab avec implémentation complète

## 🚀 Étapes Clés

1. Préparation des données temporelles (tri chronologique)
2. Normalisation avec MinMaxScaler
3. Création des séquences (windowing 24h)
4. Split train/test temporel (80/20)
5. Architecture LSTM
6. Entraînement et monitoring
7. Évaluation (graphiques Réel vs Prédit)
---

**Auteur** : khaoula esioudi  
**Date** : Décembre 2024
