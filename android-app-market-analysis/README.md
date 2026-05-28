# 📱 Android App Market Analysis — Google Play Store

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualisation-4C72B0?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **dual-dataset EDA project** on the Google Play Store — cleaning, categorising, and analysing 10,000+ apps and user reviews to understand app market dynamics, category distribution, pricing models, install patterns, and user sentiment trends.

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Datasets](#datasets)
- [Project Pipeline](#project-pipeline)
- [Features & Analysis Performed](#features--analysis-performed)
- [Tech Stack](#tech-stack)
- [Visualisations](#visualisations)
- [Setup & Usage](#setup--usage)
- [Developer](#developer)

---

## 📌 About the Project

This project analyses the Google Play Store ecosystem using two datasets — app metadata and user reviews. The goal is to understand what drives app success: category positioning, pricing strategy, install volume, content rating, and user sentiment.

The analysis covers full data cleaning (both datasets), category-level market share exploration, Free vs Paid performance comparison, install range segmentation, price distribution for paid apps, and sentiment polarity analysis from user reviews.

Built as part of my **Data Analytics Internship at Oasis Infobyte**.

---

## 📂 Datasets

### Dataset 1 — Google Play Store Apps
| Attribute | Details |
|-----------|---------|
| Records | 10,000+ apps |
| Columns | App, Category, Rating, Reviews, Size, Installs, Type, Price, Content Rating, Genres, Last Updated, Current Ver, Android Ver |
| Issues Cleaned | Duplicate apps, `Price` with `$` symbol, `Installs` with `,` and `+` characters, incorrect data types, missing Ratings |

### Dataset 2 — User Reviews
| Attribute | Details |
|-----------|---------|
| Columns | App, Translated_Review, Sentiment, Sentiment_Polarity, Sentiment_Subjectivity |
| Issues Cleaned | Null sentiment entries dropped before analysis |

---

## 🔄 Project Pipeline

```
1. Load Apps Dataset + Initial Inspection
        ↓
2. Load Reviews Dataset + Initial Inspection
        ↓
3. Data Cleaning — Apps Dataset
        ↓
4. Data Cleaning — Reviews Dataset
        ↓
5. Category Distribution Analysis
        ↓
6. Rating Distribution Analysis
        ↓
7. Install Range Segmentation
        ↓
8. Free vs Paid App Comparison
        ↓
9. Paid App Pricing Analysis
        ↓
10. Top Categories by Installs + Ratings
        ↓
11. Installs vs Reviews Scatter (log scale)
        ↓
12. Sentiment Analysis from User Reviews
        ↓
13. Business Insights Summary
```

---

## ✅ Features & Analysis Performed

### 1. 🧹 Data Cleaning — Apps Dataset
- Removed duplicate app entries
- Stripped `$` from `Price` column and converted to float
- Stripped `,` and `+` from `Installs` column and converted to integer
- Converted `Reviews` column from string to numeric
- Filled missing `Rating` values with column median
- Fixed data type inconsistencies across columns

---

### 2. 🧹 Data Cleaning — Reviews Dataset
- Dropped rows with null `Sentiment` values
- Prepared `Sentiment_Polarity` for analysis

---

### 3. 🗂️ Category Distribution
- Bar chart of app count per category across all 33 categories
- Identifies which categories are most saturated vs underserved
- Category-wise total install analysis

---

### 4. ⭐ Rating Distribution
- Histogram of app ratings across all apps
- Distribution shape and concentration range analysis
- Category-wise average rating comparison

---

### 5. 📦 Install Range Segmentation
Apps were bucketed into 7 install tiers:

| Tier | Range |
|------|-------|
| 1 | < 1,000 installs |
| 2 | 1,000 – 10,000 |
| 3 | 10,000 – 100,000 |
| 4 | 100,000 – 1M |
| 5 | 1M – 10M |
| 6 | 10M – 100M |
| 7 | 100M+ |

→ Bar chart shows distribution of apps across install tiers

---

### 6. 💸 Free vs Paid Analysis
- Count comparison of Free vs Paid apps
- Average rating comparison between Free and Paid
- Average installs comparison between Free and Paid
- Reveals whether paid apps outperform free ones in quality metrics

---

### 7. 💰 Paid App Pricing Analysis
- Distribution of prices for paid apps
- Box plot of pricing spread by category
- Identifies outlier pricing in specific categories

---

### 8. 🔗 Installs vs Reviews Scatter (Log Scale)
- Scatter plot of log(Installs) vs log(Reviews) coloured by Rating
- Reveals the relationship between review volume, popularity, and quality
- Log scale used to handle wide range of values (1 to 1B+)

---

### 9. 💬 Sentiment Analysis
- Merged apps dataset with reviews dataset on App name
- Sentiment distribution: Positive / Negative / Neutral
- Sentiment polarity score distribution by category
- Identifies which categories receive the most positive vs negative feedback

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, merging, grouping |
| NumPy | Numerical operations, log transforms |
| Matplotlib | Bar charts, scatter plots, histograms, subplots |
| Seaborn | Box plots, styled charts, colour palettes |

---

## 🖼️ Visualisations Generated

- Category distribution bar chart (33 categories)
- Rating distribution histogram
- Install range segmentation bar chart (7 tiers)
- Free vs Paid comparison (count, rating, installs)
- Paid app price distribution histogram
- Price box plot by category
- Installs vs Reviews log-scale scatter (coloured by Rating)
- Sentiment distribution bar chart
- Sentiment polarity distribution histogram
- Category-wise sentiment polarity box plot

---

## ⚙️ Setup & Usage

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn
```

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/android-app-market-analysis
```

**2. Add the datasets**
- Place `googleplaystore.csv` and `googleplaystore_user_reviews.csv` inside the `data/` folder
- Dataset available at: [Google Play Store Dataset — Kaggle](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

**3. Run the notebook**
```bash
jupyter notebook android_app_market_analysis.ipynb
```

---

## 👨‍💻 Developer

**Soham Gopal Pawar**
B.Sc. Computer Science (SYCS) — Bhavan's College, Mumbai
Data Analytics Intern — Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)

---

> ⭐ If you found this project useful, consider giving the repository a star!
