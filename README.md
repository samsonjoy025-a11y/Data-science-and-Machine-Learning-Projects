# Data-science-and-Machine-Learning-Capstone-Projects
# Building Insurance Claim Prediction by Joy Ifesinachi Samson

## 📖 Project Overview
This project aims to build a predictive machine learning model that determines whether a building will have at least one insurance claim during an insured period.

The model predicts the **probability of a claim** based on building characteristics such as structural and categorical features.

---

## 🎯 Problem Statement
Given building-related data, predict:
- **1** → Building has at least one insurance claim  
- **0** → Building has no insurance claim  

This is a **binary classification problem** with an imbalanced target variable.

---

## 📊 Dataset Description
- Target variable: **Claim**
- Numerical features: Building-related measurements
- Categorical features: Building classifications
- Missing values were handled during preprocessing

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights from EDA:
- The dataset is **imbalanced**, with ~77% non-claim buildings and ~23% claim buildings.
- Older buildings tend to have a higher probability of insurance claims.
- Certain categorical features show higher claim rates.
- Outliers were observed in some numerical features.

Visualizations include:
- Feature distributions (histograms & boxplots)
- Categorical value counts
- Feature vs target analysis

---

## 🛠 Data Preprocessing
- Missing numerical values filled using **median**
- Missing categorical values filled using **mode**
- Categorical variables encoded using **One-Hot Encoding**
- Numerical features scaled using **StandardScaler**
- Class imbalance handled using **class weights**

---

## 🤖 Models Implemented
The  models were trained and evaluated using:
- Logistic Regression (baseline)


---

## 📈 Model Evaluation
Evaluation metrics used:
- Precision


The logistic regression  model was selected based on the type of dataset I worked with which is a binary dataset  
---

## 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone <your-repo-link>
