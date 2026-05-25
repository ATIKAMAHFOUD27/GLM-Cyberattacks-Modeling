# 🛡️ Modélisation de la Fréquence des Cyberattaques via les Modèles Linéaires Généralisés (GLM)

## 📌 Présentation du Projet
Avec l'explosion de la transformation numérique, la quantification des cyber-risques est devenue un enjeu stratégique pour les organisations et les assureurs. L'objectif de ce projet est de modéliser la **fréquence des cyberattaques (violations de données)** en utilisant des approches de comptage avancées issues des **Modèles Linéaires Généralisés (GLM)**.

Ce travail met en œuvre un pipeline complet de Data Science : de l'analyse exploratoire rigoureuse à la gestion de la surdispersion dans les données de comptage.

---

## 🛠️ Stack Technique & Outils
* **Langage :** Python 🐍
* **Environnement :** Jupyter Notebook
* **Librairies Clés :**
  * `pandas` & `numpy` : Manipulation et préparation des données.
  * `matplotlib` & `seaborn` : Visualisation et analyses descriptives.
  * `statsmodels` : Implémentation, estimation et diagnostic des modèles GLM.
  * `scipy.stats` : Tests statistiques et ajustements de lois.

---

## 📊 Méthodologie et Étapes du Projet

### 1. Analyse Exploratoire des Données (EDA)
* **Nettoyage :** Traitement des valeurs manquantes et formatage des variables temporelles/catégorielles.
* **Analyse de la variable cible :** Étude de la distribution de la fréquence des attaques (comptage).
* **Visualisation :** Identification des tendances macroéconomiques, sectorielles et temporelles des violations de données.

### 2. Modélisation Statistique (GLM)
Pour capturer la nature des données de comptage, plusieurs familles de modèles ont été implémentées et comparées :
* **Régression de Poisson :** Modèle de référence (baseline) utilisant une fonction de lien logarithmique.
* **Régression Quasi-Poisson :** Introduite pour corriger et ajuster la variance en présence de surdispersion ($Var(X) > E(X)$).
* **Modèle Binomial Négatif :** Modèle alternatif robuste pour modéliser des données hautement dispersées avec une structure de variance quadratique.

### 3. Évaluation et Sélection de Modèles
* Analyse des résidus de déviance (Deviance residuals).
* Comparaison des critères d'information (**AIC**, **BIC**).
* Interprétation des coefficients (rapports de taux d'incidence / *Incidence Rate Ratios* - IRR) pour identifier les facteurs de risque majeurs.

---

## 📁 Organisation du Dépôt
* 📄 `regression_poisson_cyberattaques.ipynb` : Notebook Jupyter contenant l'intégralité du code source commenté et exécuté.
* 📊 `data/` : Répertoire contenant le jeu de données d'analyse (violations de données).
* 📝 `README.md` : Présentation générale du projet.

---

## 👥 Auteurs
* **MAHFOUD Atika** - Étudiante Ingénieure en Statistique et Big Data à l'**INSEA**
* **HAYEB Hajar** - Étudiante Ingénieure en Statistique et Big Data à l'**INSEA**

---
💡 *Ce projet a été réalisé dans le cadre du module de Modèles Linéaires Généralisés (GLM).*
