 Heart 

👥 Auteur
**[ameni dhaouadi]** - Data Scientist

**Encadré par :** M. Abdallah Khemais  
**Date :** Avril 2026  
**Module :** Machine Learning

---

## 📋 Table des matières
- [Problématique](#-problématique)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Pipeline ML](#-pipeline-ml)
- [Résultats](#-résultats)
- [Structure du projet](#-structure-du-projet)
- [Conclusion](#-conclusion)

---

## 🎯 Problématique

### Contexte
Les maladies cardiovasculaires sont la **première cause de mortalité** dans le monde (17,9 millions de décès par an selon l'OMS).

### Objectif business
Aider les professionnels de santé à **identifier les patients à risque** de maladie cardiaque sur la base d'examens simples (cliniques et électrocardiogrammes).

### Objectif technique
Construire un modèle de **classification binaire supervisée** pour prédire la présence d'une maladie cardiaque.

### Variable cible
| Valeur | Signification |
|--------|---------------|
| 0 | Patient sain (absence de maladie) |
| 1 | Patient malade (présence de maladie) |

### Métrique d'évaluation
Les **faux négatifs** (patient malade prédit sain) sont plus graves médicalement.  
➜ **Métrique principale : Recall (sensibilité)**  
➜ **Métrique secondaire : F1-Score**

---

## 📊 Dataset

### Source
**Stanford Heart Disease Dataset** - Données cliniques réelles anonymisées

### Caractéristiques
| Propriété | Valeur |
|-----------|--------|
| Nombre de patients | 918 |
| Nombre de features | 11 |
| Type de problème | Classification binaire |
| Équilibre des classes | 55% malades / 45% sains |

### Variables descriptives

| Feature | Description | Type |
|---------|-------------|------|
| Age | Âge du patient (années) | Numérique |
| Sex | Sexe (M/F) | Catégoriel |
| ChestPainType | Type de douleur thoracique (ATA, NAP, ASY, TA) | Catégoriel |
| RestingBP | Pression artérielle au repos (mm Hg) | Numérique |
| Cholesterol | Taux de cholestérol (mg/dL) | Numérique |
| FastingBS | Glycémie à jeun > 120 mg/dL (0/1) | Binaire |
| RestingECG | Résultats ECG (Normal, ST, LVH) | Catégoriel |
| MaxHR | Fréquence cardiaque maximale atteinte | Numérique |
| ExerciseAngina | Angine provoquée par l'effort (Y/N) | Binaire |
| Oldpeak | Dépression du segment ST | Numérique |
| ST_Slope | Pente du segment ST (Up, Flat, Down) | Catégoriel |
| **HeartDisease** | **Cible (0/1)** | **Binaire** |

---

## Installation


### Cloner le dépôt
```bash
git clone https://github.com/VOTRE-NOM/heart.git
cd heart-disease-prediction
