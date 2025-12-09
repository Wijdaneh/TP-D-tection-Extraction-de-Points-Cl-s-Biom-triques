# 🧬 TP -- Détection & Extraction de Points Clés Biométriques

## ⭐ Présentation du Projet

Ce projet implémente une pipeline complète de **traitement biométrique
multimodal** incluant :

-   🖼️ **Reconnaissance faciale**\
-   ✋ **Analyse d'empreintes digitales**\
-   🎤 **Analyse vocale**

L'objectif est d'extraire des **points clés**, calculer des **empreintes
numériques uniques**, générer des **visualisations**, et produire un
**système sécurisé d'encodage biométrique** (type *fuzzy vault*).

------------------------------------------------------------------------

## 🚀 Fonctionnalités principales

### 🔍 1. Détection & Prétraitement

-   Détection de visages (Haar Cascades / DNN)
-   Normalisation & alignement
-   Filtrage des empreintes digitales
-   Nettoyage des signaux audio

### 🎯 2. Extraction des Feature Vectors

-   Landmarks faciaux
-   Minuties d'empreintes (simplifiées)
-   Coefficients MFCC pour la voix
-   PCA & réduction dimensionnelle

### 📊 3. Visualisations

-   Heatmaps de similarité\
-   PCA 2D par modalité\
-   Histogrammes de qualité\
-   Courbes de distances inter-individuelles

### 🔐 4. Sécurisation des Données

-   Implémentation d'un mini **fuzzy vault**
-   Génération de fichiers vault (.csv)
-   Extraction et sauvegarde chiffrée simplifiée

### 📝 5. Rapports Automatiques

-   `summary_report.txt`
-   `system_report.txt`
-   Logs d'exécution détaillés

------------------------------------------------------------------------

## 📂 Arborescence du projet

    TP4/
    │
    ├── Data/
    │   ├── faces/
    │   ├── fingerprint/
    │   └── voices/
    │
    ├── outputs/
    │   ├── visualisations (*.png)
    │   ├── features (*.csv)
    │   ├── secured/*.csv
    │   └── reports/*.txt
    │
    └── tp4_biometric_v3.ipynb

------------------------------------------------------------------------

## 🛠️ Technologies

  Catégorie          Outils
  ------------------ ----------------------------
  Traitement image   OpenCV, scikit-image
  Audio              Librosa
  Machine Learning   Scikit-learn
  Visualisation      Matplotlib, Seaborn
  Data               NumPy, Pandas
  Dev                Python 3, Jupyter Notebook

------------------------------------------------------------------------

## ▶️ Exécution du projet

### 1️⃣ Installer les dépendances

``` bash
pip install -r requirements.txt
```

### 2️⃣ Ajouter les données biométriques

Placer les images/audio dans :

    TP4/Data/

### 3️⃣ Lancer le Notebook

``` bash
jupyter notebook TP4/tp4_biometric_v3.ipynb
```

### 4️⃣ Consulter les résultats

Ils se trouvent dans :

    TP4/outputs/

------------------------------------------------------------------------

## 📈 Exemple de Résultats

-   Heatmap de similarité faciale\
-   Projection PCA fingerprint\
-   Analyse MFCC audio\
-   Rapports de performance\
-   Vaults sécurisés en CSV

------------------------------------------------------------------------

## 🧪 Améliorations futures (Roadmap)

-   🔧 Ajout de réseaux neuronaux (CNN)
-   🧠 Détection biométrique via Deep Learning
-   🔐 Implémentation avancée du fuzzy vault
-   🌐 API Flask pour l'extraction biométrique
-   🎨 Dashboard React pour visualisation temps réel

------------------------------------------------------------------------

## 📜 Licence

Ce projet est sous **MIT License**.

------------------------------------------------------------------------

## 👩‍💻 Auteur

**Wijdane Hachani**\
Étudiante en cybersécurité et confiance numérique\
GitHub : https://github.com/Wijdaneh
