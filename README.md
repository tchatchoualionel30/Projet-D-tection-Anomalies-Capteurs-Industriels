# 🏭 Détection d'Anomalies sur Capteurs Industriels

**Projet de Maintenance Prédictive** conçu pour identifier les comportements thermiques anormaux et anticiper les pannes sur une pompe hydraulique industrielle.

## 🎯 Objectif et Performance
- **Objectif :** Isoler les anomalies thermiques avant ou pendant une défaillance matérielle.
- **Algorithme :** `IsolationForest` (Machine Learning Non-Supervisé).
- **Performance atteinte :** Taux de détection (Recall) de **95.9%** sur les pannes réelles.

## 📊 Données
Le projet utilise le dataset Kaggle de référence **"Pump Sensor Data"**. 
Après un nettoyage des données et un ciblage des capteurs thermiques pertinents (capteurs 00 à 04), le jeu de données final contient 220 261 relevés.
- **Feature Engineering :** Application de moyennes mobiles (Rolling Means sur 1h) pour lisser le bruit thermique et capter l'inertie des températures.

## 🛠️ Technologies Utilisées
- **Python 3**
- **Scikit-Learn** (Modélisation via Isolation Forest)
- **Pandas / Numpy** (Manipulation de séries temporelles)
- **Matplotlib / Seaborn** (Visualisation des matrices de confusion et des séries temporelles)

## 🚀 Utilisation
1. Clonez ce dépôt.
2. Téléchargez le fichier `sensor.csv` depuis Kaggle et placez-le à la racine.
3. Installez les dépendances via `pip install -r requirements.txt`.
4. Exécutez le notebook Jupyter / Colab.
