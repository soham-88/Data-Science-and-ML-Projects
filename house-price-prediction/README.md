# 🏠 House Price Prediction using Linear Regression

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **complete end-to-end Machine Learning pipeline** to predict California median house prices using Linear Regression — covering geographic visualisation, feature engineering, StandardScaler preprocessing, model training, residual analysis, permutation-based feature importance, and 5-fold cross-validation on the California Housing dataset.

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Project Pipeline](#project-pipeline)
- [Features](#features)
- [Model Performance](#model-performance)
- [Feature Engineering](#feature-engineering)
- [Tech Stack](#tech-stack)
- [Visualisations](#visualisations)
- [Setup & Usage](#setup--usage)
- [Developer](#developer)

---

## 📌 About the Project

This project builds a predictive model to estimate median house prices in California using the California Housing dataset. It demonstrates a full ML workflow — from raw data inspection to cross-validated model evaluation.

The project includes geographic scatter visualisation (latitude/longitude), derived feature engineering, label encoding for categorical features, StandardScaler normalisation, Linear Regression training, and a detailed evaluation including actual vs predicted plots, residual distribution analysis, and coefficient-based feature importance.

Built as part of my **Data Analytics Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Source | California Housing Dataset |
| Records | 20,640 rows |
| Features | 10 columns (longitude, latitude, housing_median_age, total_rooms, total_bedrooms, population, households, median_income, ocean_proximity, median_house_value) |
| Target Variable | `median_house_value` |
| Missing Values | 207 missing in `total_bedrooms` — filled with median |
| Outputs | `housing_cleaned.csv`, `predictions.csv` |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. Descriptive Statistics & Distribution Analysis
        ↓
3. Geographic Visualisation (lat/long scatter)
        ↓
4. Ocean Proximity Analysis
        ↓
5. Correlation Heatmap (with encoded features)
        ↓
6. Data Preprocessing (null imputation + encoding)
        ↓
7. Feature Engineering (3 derived features)
        ↓
8. Train-Test Split (80/20) + StandardScaler
        ↓
9. Linear Regression Model Training
        ↓
10. Model Evaluation (R², RMSE, MAE)
        ↓
11. Actual vs Predicted + Residual Analysis
        ↓
12. Feature Importance (Coefficients + Permutation)
        ↓
13. 5-Fold Cross Validation
        ↓
14. Sample Predictions Table + Export
```

---

## ✅ Features

### 1. 🧹 Data Preprocessing
- Filled 207 missing `total_bedrooms` values using median imputation
- Label Encoded `ocean_proximity` categorical column (5 categories: NEAR BAY, <1H OCEAN, INLAND, NEAR OCEAN, ISLAND)
- Applied `StandardScaler` to normalise all features before model training

---

### 2. 🔧 Feature Engineering
Three new derived features were created from existing columns:

| New Feature | Formula | Purpose |
|-------------|---------|---------|
| `rooms_per_household` | total_rooms / households | Avg rooms per household |
| `bedrooms_per_room` | total_bedrooms / total_rooms | Bedroom density ratio |
| `population_per_household` | population / households | Crowding metric |

These engineered features improve model interpretability and capture more meaningful relationships than raw room/population counts.

---

### 3. 🗺️ Geographic Visualisation
- Latitude/Longitude scatter plot coloured by `median_house_value` using RdYlGn colormap
- Population density scatter using bubble size
- Clearly shows coastal premium — houses near the ocean have higher values

---

### 4. 🏘️ Ocean Proximity Analysis
- 3-panel analysis: App count, Average House Value, and Median House Value by ocean proximity category
- Reveals ISLAND > NEAR BAY > NEAR OCEAN > <1H OCEAN > INLAND price ordering

---

### 5. 📐 Model Training
- **Algorithm:** Linear Regression (Scikit-learn)
- **Split:** 80% Training / 20% Test (random_state=42)
- **Scaling:** StandardScaler fitted on training set only, transformed on both sets

---

### 6. 📊 Model Evaluation
Full evaluation suite including:
- R² Score (Train + Test)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Actual vs Predicted scatter plot with perfect prediction line
- Residuals distribution histogram
- Residuals vs Predicted scatter plot (heteroscedasticity check)
- Residuals vs Feature (median_income) scatter

---

### 7. 🔬 Feature Importance
- **Coefficient-based importance** — absolute value of model coefficients ranked
- **Permutation importance** — measures actual impact on R² when feature is shuffled
- Both shown as horizontal bar charts for comparison

---

### 8. ✅ 5-Fold Cross Validation
- Cross-validated R² scores across 5 folds
- Mean CV R² reported for robust performance estimate
- CV score bar chart with mean line overlay

---

## 📈 Model Performance

| Metric | Train Set | Test Set |
|--------|-----------|---------|
| R² Score | Reported in notebook | Reported in notebook |
| RMSE | Reported in notebook | Reported in notebook |
| MAE | Reported in notebook | Reported in notebook |
| CV Mean R² | 5-Fold | Reported in notebook |

> Run the notebook to see the exact values computed on the dataset.

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, feature engineering |
| NumPy | Numerical operations, array handling |
| Matplotlib | Scatter plots, histograms, bar charts, subplots |
| Seaborn | Heatmap, styled distribution plots |
| Scikit-learn | Train-test split, StandardScaler, LinearRegression, metrics, cross_val_score, permutation_importance |

---

## 🖼️ Visualisations Generated

- 3×3 feature distribution histograms (9 features)
- Geographic house value scatter (lat/long + colormap)
- Geographic population density scatter
- 3-panel Ocean Proximity analysis
- Correlation heatmap (9 features, encoded)
- Median income vs house value scatter (coloured by age)
- House value distribution (histogram + log scale)
- Actual vs Predicted scatter with diagonal line
- Residuals distribution histogram
- Residuals vs Predicted scatter
- Residuals vs Median Income scatter
- Coefficient importance horizontal bar chart
- Permutation importance horizontal bar chart
- 5-fold CV scores bar chart with mean line

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
cd Data-Science-and-ML-Projects/house-price-prediction
```

**2. Add the dataset**
- Place `housing.csv` inside the `data/` folder
- Dataset available at: [California Housing Dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

**3. Run the notebook**
```bash
jupyter notebook house_price_prediction.ipynb
```

**4. View outputs**
- Cleaned dataset: `data/housing_cleaned.csv`
- Predictions: `data/predictions.csv`
- All charts render inline in the notebook

---

## 👨‍💻 Developer

**Soham Gopal Pawar**
B.Sc. Computer Science (SYCS) — Bhavan's College, Mumbai
Data Analytics Intern — Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

---

> ⭐ If you found this project useful, consider giving the repository a star!
