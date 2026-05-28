# 🌸 Iris Flower Classification

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **multi-class classification project** that identifies iris flower species (Setosa, Versicolor, Virginica) from sepal and petal measurements using a Random Forest Classifier — one of the most well-known benchmark datasets in machine learning.

---

## 📋 Table of Contents
- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Project Pipeline](#project-pipeline)
- [Features](#features)
- [Model Performance](#model-performance)
- [Tech Stack](#tech-stack)
- [Setup & Usage](#setup--usage)
- [Developer](#developer)

---

## 📌 About the Project

This project builds a supervised classification model to identify iris species using 4 numerical features. It demonstrates the complete ML classification workflow — EDA, visualisation, model training, and evaluation using confusion matrix and classification report.

Built as part of my **Data Science Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Source | Iris Dataset (UCI / Scikit-learn built-in) |
| Records | 150 rows |
| Features | Sepal Length, Sepal Width, Petal Length, Petal Width |
| Target | Species: Setosa, Versicolor, Virginica |
| Classes | 3 (50 samples per class) |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. EDA — Feature Distributions & Pair Plots
        ↓
3. Feature Correlation Heatmap
        ↓
4. Train-Test Split (80/20)
        ↓
5. Random Forest Classifier Training
        ↓
6. Prediction + Evaluation
        ↓
7. Confusion Matrix + Classification Report
        ↓
8. Feature Importance Analysis
```

---

## ✅ Features

### 1. 📊 Exploratory Data Analysis
- Pair plot to visualise class separation across all feature combinations
- Box plots per feature coloured by species
- Identifies that Petal Length and Petal Width are the strongest discriminators

### 2. 🌲 Random Forest Classifier
- Ensemble of decision trees for robust classification
- Handles multi-class output natively
- Outputs per-class precision, recall, F1-score

### 3. 📈 Model Evaluation
- Accuracy Score
- Confusion Matrix (heatmap)
- Classification Report (Precision, Recall, F1 per class)
- Feature Importance bar chart

---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| Algorithm | Random Forest Classifier |
| Classes | 3 (Setosa, Versicolor, Virginica) |
| Accuracy | High (typically 95–100% on this dataset) |
| Split | 80% Train / 20% Test |

---

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn`

---

## ⚙️ Setup & Usage

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/iris-flower-classification
jupyter notebook iris_classification.ipynb
```

---

## 👨‍💻 Developer

**Soham Gopal Pawar** — B.Sc. CS, Bhavan's College Mumbai | Data Science Intern @ Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

> ⭐ If you found this project useful, consider giving the repository a star!
