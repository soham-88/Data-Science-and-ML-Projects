# 📧 Email Spam Detection using NLP

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-TF--IDF-9B59B6?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

A **Natural Language Processing project** that builds a binary email spam detection system using TF-IDF vectorisation and a Multinomial Naive Bayes classifier — achieving approximately **98% classification accuracy** on real email data.

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

This project builds a spam detection system that classifies emails as **Spam** or **Ham (Legitimate)** using classic NLP techniques.

The pipeline covers text preprocessing, TF-IDF feature extraction, Multinomial Naive Bayes training, and thorough evaluation using accuracy score, confusion matrix, and classification report. It demonstrates a practical, deployable NLP classification workflow.

Built as part of my **Data Science Internship at Oasis Infobyte**.

---

## 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Type | Labelled email dataset (Spam / Ham) |
| Labels | `spam` → 1, `ham` → 0 |
| Features | Raw email text |
| Source | UCI SMS Spam Collection / email dataset |

---

## 🔄 Project Pipeline

```
1. Data Loading & Inspection
        ↓
2. Label Encoding (spam=1, ham=0)
        ↓
3. Text Preprocessing (lowercase, punctuation, stopwords)
        ↓
4. TF-IDF Vectorisation
        ↓
5. Train-Test Split (80/20)
        ↓
6. Multinomial Naive Bayes Training
        ↓
7. Prediction + Evaluation
        ↓
8. Confusion Matrix + Classification Report
        ↓
9. Sample Predictions
```

---

## ✅ Features

### 1. 🧹 Text Preprocessing
- Converted all text to lowercase
- Removed punctuation and special characters
- Removed English stopwords
- Prepared clean text corpus for vectorisation

---

### 2. 🔢 TF-IDF Vectorisation
**TF-IDF (Term Frequency–Inverse Document Frequency)** converts raw email text into numerical feature vectors:

| Component | What It Measures |
|-----------|-----------------|
| **TF (Term Frequency)** | How often a word appears in this email |
| **IDF (Inverse Document Frequency)** | How rare the word is across all emails |
| **TF-IDF Score** | High for words that are frequent in this email but rare across all emails — these are the discriminating words |

Words like "free", "winner", "click here", "offer" get high TF-IDF scores in spam — this is what the model learns from.

---

### 3. 🤖 Multinomial Naive Bayes Classifier
- Ideal for text classification with TF-IDF features
- Applies Bayes' theorem with independence assumption across word features
- Fast training, interpretable, and highly effective on text data
- Trained on 80% of the dataset, evaluated on 20%

---

### 4. 📊 Model Evaluation
- **Accuracy Score** — overall classification accuracy
- **Confusion Matrix** — True Positives, True Negatives, False Positives, False Negatives
- **Classification Report** — Precision, Recall, F1-Score for both Spam and Ham classes
- **Visualised Confusion Matrix** — heatmap format

---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| Accuracy | ~98% |
| Classification | Spam vs Ham (binary) |
| Vectoriser | TF-IDF |
| Model | Multinomial Naive Bayes |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| Python 3.x | Core language |
| Pandas | Data loading and label encoding |
| NumPy | Array operations |
| Scikit-learn | TF-IDF Vectoriser, Naive Bayes, train_test_split, metrics |
| Matplotlib / Seaborn | Confusion matrix heatmap visualisation |

---

## ⚙️ Setup & Usage

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/soham-88/Data-Science-and-ML-Projects.git
cd Data-Science-and-ML-Projects/email-spam-detection
```

**2. Add the dataset**
- Place the spam/ham email dataset CSV inside the `data/` folder

**3. Run the notebook**
```bash
jupyter notebook email_spam_detection.ipynb
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
