# Building Insurance Claim Prediction

## 📌 Project Overview
This project aims to build a predictive model that estimates the probability of a building having at least one insurance claim during its insured period. The prediction is based on building characteristics.

The task is framed as a binary classification problem:
- **1**: Building has at least one claim
- **0**: Building has no claim

---

## 📊 Dataset Description
The dataset contains building-level information including numerical and categorical features describing structural, usage, and location attributes.

The target variable **Claim** is imbalanced, with fewer buildings experiencing insurance claims.

---

## 🧹 Data Cleaning & Preprocessing
The following preprocessing steps were applied:
- Missing values handled using:
  - Mean imputation for numerical features
  - Most frequent value imputation for categorical features
- Categorical variables encoded using One-Hot Encoding
- Numerical features scaled using StandardScaler
- Target leakage was avoided by applying preprocessing only within pipelines

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was conducted to understand feature distributions and their relationship with insurance claims:
- Target distribution analysis revealed class imbalance
- Numerical features showed skewness, motivating feature scaling
- Categorical features were analyzed using frequency counts
- Claim rates were compared across categorical feature levels

Key insights from EDA informed preprocessing and modeling choices.

---

## 🤖 Modeling Approach
Two machine learning models were implemented and compared:

### 1. Logistic Regression (Baseline Model)
- Used as an interpretable baseline
- Class imbalance handled using `class_weight='balanced'`

### 2. Random Forest Classifier
- Captures non-linear relationships between features
- Robust to outliers and feature interactions
- Class imbalance handled using balanced class weights

All models were implemented using Scikit-learn pipelines for reproducibility and to prevent data leakage.

---

## 📈 Model Evaluation
Models were evaluated using the following metrics:
- ROC-AUC
- Precision
- Recall
- F1-score

The Random Forest model achieved the best overall performance, particularly in identifying buildings at higher risk of insurance claims.

---

## ✅ Conclusion
After comparing multiple models and preprocessing strategies, Random Forest was selected as the final model due to its superior predictive performance and robustness.

---

## 🛠️ Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 📂 Project Structure


---

## 👤 Author
**Joy Samson**
