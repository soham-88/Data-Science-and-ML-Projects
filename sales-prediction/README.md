# 📈 Sales Prediction using Linear Regression

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **regression ML project** that predicts product sales based on advertising spend across TV, Radio, and Newspaper channels — using Linear Regression to uncover which advertising channel drives the most revenue impact.

---

## 📋 Table of Contents
- [About the Project](#about-the-project-2)
- [Dataset](#dataset-2)
- [Project Pipeline](#project-pipeline-2)
- [Features](#features-1)
- [Model Performance](#model-performance-1)
- [Tech Stack](#tech-stack-2)
- [Setup & Usage](#setup--usage-2)
- [Developer](#developer-2)

---

## 📌 About the Project

This project models the relationship between advertising spend (TV, Radio, Newspaper) and product sales using Linear Regression. The analysis identifies which advertising channel has the highest return on investment and builds a model that can forecast sales from a given advertising budget.

Built as part of my **Data Science Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Records | 200 rows |
| Features | TV (ad spend in $000s), Radio (ad spend in $000s), Newspaper (ad spend in $000s) |
| Target | Sales (in units/thousands) |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. EDA — Feature Distributions
        ↓
3. Scatter Plots — Each Channel vs Sales
        ↓
4. Correlation Heatmap
        ↓
5. Train-Test Split (80/20)
        ↓
6. Linear Regression Training
        ↓
7. Model Evaluation (R², MAE, RMSE)
        ↓
8. Actual vs Predicted Visualisation
        ↓
9. Coefficient Analysis — Channel ROI
```

---

## ✅ Features

### 1. 📊 Channel vs Sales Analysis
- Scatter plots for TV vs Sales, Radio vs Sales, Newspaper vs Sales
- Identifies which channels have strongest linear relationship with sales
- TV typically shows the highest correlation

### 2. 🔥 Correlation Heatmap
- Heatmap across all 4 variables (TV, Radio, Newspaper, Sales)
- Confirms TV and Radio as primary sales drivers

### 3. 📐 Linear Regression Model
- Trained on 80% of data, evaluated on 20%
- Coefficients reveal the marginal impact of each ₹1 spent per channel
- Intercept represents baseline sales with zero advertising spend

### 4. 📈 Model Evaluation
- R² Score — how well the model explains sales variance
- MAE — average absolute prediction error
- RMSE — error metric penalising larger mistakes
- Actual vs Predicted scatter plot

### 5. 💡 Coefficient Insights
- TV coefficient: highest positive impact per unit spend
- Newspaper: lowest or near-zero impact (often statistically insignificant)
- Informs real-world budget allocation decisions

---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| Algorithm | Linear Regression |
| Features | TV, Radio, Newspaper |
| Target | Sales |
| Split | 80% Train / 20% Test |

---

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn`

---

## ⚙️ Setup & Usage

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/sales-prediction
jupyter notebook sales_prediction.ipynb
```

Dataset available at: [Advertising Dataset — Kaggle](https://www.kaggle.com/datasets/bumba5341/advertisingcsv)

---

## 👨‍💻 Developer

**Soham Gopal Pawar** — B.Sc. CS, Bhavan's College Mumbai | Data Science Intern @ Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

> ⭐ If you found this project useful, consider giving the repository a star!
