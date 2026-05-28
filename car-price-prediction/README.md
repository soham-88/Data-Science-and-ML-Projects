# 🚗 Car Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **regression-based Machine Learning project** that predicts used car selling prices based on features including fuel type, mileage, transmission, seller type, and vehicle age — achieving an **R² score of approximately 0.88** using a Random Forest Regressor.

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

This project predicts the selling price of used cars using a Random Forest Regressor. It covers the complete ML pipeline — data exploration, preprocessing, feature engineering, encoding, model training, and evaluation.

The dataset contains real-world used car listings with attributes that directly affect resale value. The model learns these patterns and predicts prices with strong R² accuracy.

Built as part of my **Data Science Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Features | Car Name, Year, Selling Price, Present Price, Kms Driven, Fuel Type, Seller Type, Transmission, Owner |
| Target Variable | `Selling_Price` |
| Categorical Features | Fuel Type (Petrol/Diesel/CNG), Seller Type (Dealer/Individual), Transmission (Manual/Automatic) |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. Exploratory Data Analysis
        ↓
3. Feature Engineering (Car Age from Year)
        ↓
4. Categorical Encoding (Label Encoding)
        ↓
5. Feature Selection (drop irrelevant columns)
        ↓
6. Train-Test Split (80/20)
        ↓
7. Random Forest Regressor Training
        ↓
8. Model Evaluation (R², MAE, RMSE)
        ↓
9. Feature Importance Analysis
        ↓
10. Actual vs Predicted Visualisation
```

---

## ✅ Features

### 1. 🔧 Feature Engineering
- Created `Car_Age` = Current Year − `Year` column
- Dropped the original `Year` and `Car_Name` columns (not useful for prediction)
- Age is a stronger predictor than the raw manufacturing year

---

### 2. 🔢 Categorical Encoding
Label Encoded 3 categorical columns:

| Column | Values |
|--------|--------|
| Fuel_Type | Petrol, Diesel, CNG |
| Seller_Type | Dealer, Individual |
| Transmission | Manual, Automatic |

---

### 3. 🌲 Random Forest Regressor
- Ensemble of decision trees — robust to overfitting
- Handles non-linear relationships between features and price
- Outputs feature importance scores automatically
- Trained with 80/20 train-test split (random_state=42)

---

### 4. 📊 Model Evaluation
- R² Score — proportion of variance explained
- Mean Absolute Error (MAE) — average absolute prediction error
- Root Mean Squared Error (RMSE) — penalises large errors more
- Actual vs Predicted scatter plot with diagonal reference line

---

### 5. 📌 Feature Importance
- Bar chart of Random Forest feature importance scores
- Identifies which features most strongly influence car price prediction
- `Present_Price`, `Car_Age`, and `Kms_Driven` typically rank highest

---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| R² Score | ~0.88 |
| Algorithm | Random Forest Regressor |
| Train-Test Split | 80% / 20% |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, feature engineering |
| NumPy | Numerical operations |
| Matplotlib / Seaborn | Visualisations, feature importance charts |
| Scikit-learn | RandomForestRegressor, train_test_split, metrics |

---

## ⚙️ Setup & Usage

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/car-price-prediction
```

**2. Add the dataset**
- Place the car dataset CSV inside the `data/` folder
- Dataset available at: [Car Price Dataset — Kaggle](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

**3. Run the notebook**
```bash
jupyter notebook car_price_prediction.ipynb
```

---

## 👨‍💻 Developer

**Soham Gopal Pawar**
B.Sc. Computer Science (SYCS) — Bhavan's College, Mumbai
Data Science Intern — Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

---

> ⭐ If you found this project useful, consider giving the repository a star!
