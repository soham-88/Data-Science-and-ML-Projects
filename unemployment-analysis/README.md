# 📉 Unemployment Analysis

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

An **EDA project** analysing India's unemployment rate trends during the COVID-19 period — visualising state-wise and region-wise patterns in estimated employment, labour participation rate, and unemployment rate across time.

---

## 📋 Table of Contents
- [About the Project](#about-the-project-1)
- [Dataset](#dataset-1)
- [Project Pipeline](#project-pipeline-1)
- [Analysis Performed](#analysis-performed)
- [Key Insights](#key-insights)
- [Tech Stack](#tech-stack-1)
- [Setup & Usage](#setup--usage-1)
- [Developer](#developer-1)

---

## 📌 About the Project

This project performs exploratory data analysis on India's unemployment dataset to uncover how COVID-19 affected employment across states and regions. The analysis focuses on the sharp unemployment spike during the April–May 2020 lockdown period, followed by partial recovery trends.

Built as part of my **Data Science Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Source | CMIE (Centre for Monitoring Indian Economy) |
| Columns | Region (State), Date, Frequency, Estimated Unemployment Rate (%), Estimated Employed, Estimated Labour Participation Rate (%), Area (Rural/Urban) |
| Period | 2019–2020 (covers pre and post COVID lockdown) |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. Data Cleaning (date formatting, null handling)
        ↓
3. Overall Unemployment Rate Trend (time series)
        ↓
4. State-Wise Unemployment Rate Analysis
        ↓
5. Region-Wise Comparison (Rural vs Urban)
        ↓
6. Labour Participation Rate Analysis
        ↓
7. Estimated Employment Trend
        ↓
8. COVID-19 Impact: Pre vs Post Lockdown Comparison
        ↓
9. Correlation Analysis
        ↓
10. Key Insights Summary
```

---

## ✅ Analysis Performed

### 1. 📈 Time Series — National Unemployment Trend
- Monthly unemployment rate plotted across the full dataset period
- Clear visualisation of the COVID-19 spike (April–May 2020)
- Recovery trend post-lockdown

### 2. 🗺️ State-Wise Analysis
- Bar chart of average unemployment rate by state
- Identifies highest and lowest unemployment states
- Horizontal bar chart sorted by unemployment rate

### 3. 🌍 Rural vs Urban Comparison
- Side-by-side unemployment rate comparison between rural and urban areas
- Reveals differential COVID impact across area types

### 4. 💼 Labour Participation Rate
- Trend analysis of labour participation alongside unemployment
- Shows whether unemployment rise was due to job loss or workforce exit

### 5. 📊 Correlation Heatmap
- Relationships between Unemployment Rate, Estimated Employed, and Labour Participation Rate

---

## 💡 Key Insights

- Unemployment rate spiked sharply in April–May 2020 during the national lockdown
- Urban areas saw a more sudden spike; rural areas saw a lagged but sustained impact
- States with higher labour participation rates showed faster recovery post-lockdown
- Post-lockdown months showed gradual normalisation but not full pre-COVID levels

---

## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn`

---

## ⚙️ Setup & Usage

```bash
pip install pandas numpy matplotlib seaborn
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/unemployment-analysis
jupyter notebook unemployment_analysis.ipynb
```

---

## 👨‍💻 Developer

**Soham Gopal Pawar** — B.Sc. CS, Bhavan's College Mumbai | Data Science Intern @ Oasis Infobyte

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soham-pawar-984b32319/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/soham-88)
