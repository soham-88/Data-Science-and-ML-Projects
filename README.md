# 🚀 Data Science & Machine Learning Projects

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A collection of **8 end-to-end Data Science and Machine Learning projects** built during my Data Science Internship at **Oasis Infobyte** and Data Analytics Internship at **Oasis Infobyte**. Each project covers the complete pipeline — data loading, cleaning, EDA, feature engineering, model training, evaluation, and visualisation.

---

## 📋 Table of Contents

- [About This Repository](#about-this-repository)
- [Projects](#projects)
- [Tech Stack](#tech-stack)
- [Repository Structure](#repository-structure)
- [Developer](#developer)

---

## 📌 About This Repository

This repository contains real-world Data Science and ML projects built using Python, covering domains including retail analytics, real estate, automotive pricing, NLP, customer segmentation, unemployment trends, sales forecasting, and mobile app market analysis.

All projects are built as Jupyter Notebooks with clean code, inline visualisations, and documented outputs.

---

## 📊 Projects

| # | Project | Domain | Type | Key Result |
|---|---------|--------|------|-----------|
| 1 | [Iris Flower Classification](#1-iris-flower-classification) | Biology | Classification | High accuracy — Random Forest |
| 2 | [Unemployment Analysis](#2-unemployment-analysis) | Economics | EDA | COVID-19 state-wise trend analysis |
| 3 | [Car Price Prediction](#3-car-price-prediction) | Automotive | Regression | R² ~0.88 — Random Forest Regressor |
| 4 | [Email Spam Detection](#4-email-spam-detection-nlp) | NLP | Classification | ~98% accuracy — Naive Bayes + TF-IDF |
| 5 | [Sales Prediction](#5-sales-prediction) | Marketing | Regression | Linear Regression on advertising data |
| 6 | [EDA on Retail Sales](#6-eda-on-retail-sales-data) | Retail | EDA + RFM | Customer segmentation + revenue analysis |
| 7 | [House Price Prediction](#7-house-price-prediction) | Real Estate | Regression | R² score + 5-fold CV on 20K records |
| 8 | [Android App Market Analysis](#8-android-app-market-analysis) | Tech | EDA | 10K+ apps analysed with sentiment |

---

## 🌸 1. Iris Flower Classification

**Type:** Multi-Class Classification
**Model:** Random Forest Classifier

Classified iris flower species (Setosa, Versicolor, Virginica) based on sepal and petal measurements using supervised ML.

→ Applied EDA, feature visualisation, and model evaluation using confusion matrix and classification report
→ [View Project](./iris-flower-classification/)

---

## 📉 2. Unemployment Analysis

**Type:** Exploratory Data Analysis
**Focus:** COVID-19 Impact on Indian Unemployment

Performed EDA on India's unemployment dataset to uncover state-wise and region-wise unemployment trends during the COVID-19 period.

→ Visualised labour participation rates, estimated employment, and unemployment rates across states and time
→ [View Project](./unemployment-analysis/)

---

## 🚗 3. Car Price Prediction

**Type:** Regression
**Model:** Random Forest Regressor
**Result:** R² ≈ 0.88

Predicted used car prices based on features including fuel type, mileage, transmission, and vehicle age. Full pipeline with feature engineering, encoding, and model evaluation.

→ [View Project](./car-price-prediction/)

---

## 📧 4. Email Spam Detection (NLP)

**Type:** Binary Classification (NLP)
**Model:** Multinomial Naive Bayes + TF-IDF
**Result:** ~98% accuracy

Built an email spam detection system using Natural Language Processing. Applied text preprocessing, TF-IDF vectorisation, and trained a classifier to distinguish spam from legitimate emails.

→ [View Project](./email-spam-detection/)

---

## 📈 5. Sales Prediction

**Type:** Regression
**Model:** Linear Regression
**Focus:** Advertising spend vs sales revenue

Predicted product sales based on advertising spend across TV, Radio, and Newspaper channels. Business-focused analysis with feature correlation and prediction insights.

→ [View Project](./sales-prediction/)

---

## 🛍️ 6. EDA on Retail Sales Data

**Type:** Advanced EDA + RFM Customer Segmentation
**Dataset:** Retail sales transactions with customer demographics

Performed comprehensive EDA on retail sales data including time series analysis, gender/age analysis, product category breakdowns, outlier detection, and RFM-based customer segmentation (Champions, Loyal, At Risk, Lost).

→ [View Project](./EDA-retail-sales/)

---

## 🏠 7. House Price Prediction

**Type:** Regression
**Model:** Linear Regression with 5-Fold Cross Validation
**Dataset:** California Housing (20,640 records, 10 features)

Built a full ML pipeline to predict California median house prices. Includes geographic visualisation, feature engineering (3 derived features), StandardScaler preprocessing, model evaluation (R², RMSE, MAE), and cross-validation.

→ [View Project](./house-price-prediction/)

---

## 📱 8. Android App Market Analysis

**Type:** EDA + Sentiment Analysis
**Dataset:** Google Play Store apps + user reviews (10,000+ entries)

Cleaned and analysed dual datasets (apps + reviews) to understand app market dynamics — category distribution, pricing, install ranges, rating patterns, and sentiment trends across user reviews.

→ [View Project](./android-app-market-analysis/)

---

## 🛠️ Tech Stack

| Category | Libraries / Tools |
|----------|------------------|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| NLP | TF-IDF Vectoriser, NLTK |
| Statistical Analysis | SciPy, Statsmodels |
| Environment | Jupyter Notebook |
| Version Control | Git, GitHub |

---

## 📂 Repository Structure

```
Data-Science-and-ML-Projects/
│
├── iris-flower-classification/
│   ├── iris_classification.ipynb
│   ├── data/
│   └── README.md
│
├── unemployment-analysis/
│   ├── unemployment_analysis.ipynb
│   ├── data/
│   └── README.md
│
├── car-price-prediction/
│   ├── car_price_prediction.ipynb
│   ├── data/
│   └── README.md
│
├── email-spam-detection/
│   ├── email_spam_detection.ipynb
│   ├── data/
│   └── README.md
│
├── sales-prediction/
│   ├── sales_prediction.ipynb
│   ├── data/
│   └── README.md
│
├── EDA-retail-sales/
│   ├── EDA_Retail_Sales.ipynb
│   ├── data/
│   └── README.md
│
├── house-price-prediction/
│   ├── house_price_prediction.ipynb
│   ├── data/
│   └── README.md
│
├── android-app-market-analysis/
│   ├── android_app_market_analysis.ipynb
│   ├── data/
│   └── README.md
│
└── README.md
```

---

## 👨‍💻 Developer

**Soham Gopal Pawar**
B.Sc. Computer Science (SYCS) — Bhavan's College, Mumbai
Data Science Intern & Data Analytics Intern — Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

---

> ⭐ If you found this repository useful, consider giving it a star!
