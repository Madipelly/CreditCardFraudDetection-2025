# 💳 Credit Card Fraud Detection Using Machine Learning

**Contributor:** Shravan Madipelly  
**Project Goal:** Predict fraudulent credit card transactions using machine learning models.

---

## 🧠 Problem Statement

The objective of this project is to build machine learning models that can accurately detect fraudulent credit card transactions. The dataset used contains anonymized customer-level transaction data collected during a research collaboration between Worldline and the Machine Learning Group.

Out of 284,807 transactions, only 492 are fraudulent, making the dataset highly imbalanced. This imbalance must be addressed to build effective predictive models.

---

## 🏦 Business Problem Overview

For banks, retaining high-value customers is a top priority. However, credit card fraud poses a serious threat to this goal, leading to:

- Substantial financial losses
- Erosion of customer trust
- Damage to institutional credibility

According to the Nilson Report, global banking fraud was projected to reach $30 billion by 2020. With the rise of digital payment systems, fraud is evolving in complexity and frequency. Machine learning offers a proactive solution to detect and prevent such frauds, reducing:

- Manual review time
- Chargebacks and penalties
- False positives that deny legitimate transactions

---

## 🔍 Understanding and Defining Fraud

Credit card fraud involves unauthorized access or manipulation of cardholder data for financial gain. Common methods include:

- Skimming (duplicating magnetic strip data)
- Manipulation or alteration of genuine cards
- Creation of counterfeit cards
- Theft or loss of credit cards
- Fraudulent telemarketing

---

## 📊 Dataset Overview

- **Source:** [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Transactions:** 284,807
- **Fraudulent Transactions:** 492 (0.172%)
- **Features:**
  - `Time`: Seconds since the first transaction
  - `Amount`: Transaction amount
  - `Class`: 1 = Fraud, 0 = Non-fraud
  - `V1` to `V28`: Principal components derived via PCA for confidentiality

---

## 🔁 Project Pipeline

### 1. Data Understanding
- Load and inspect the dataset
- Understand feature types and distributions
- Identify relevant features for modeling

### 2. Exploratory Data Analysis (EDA)
- Perform univariate and bivariate analysis
- Check for skewness and apply transformations if needed
- No Z-scaling required due to Gaussian variables

### 3. Train/Test Split
- Use stratified train/test split to preserve class distribution
- Apply k-fold cross-validation for robust validation
- Ensure minority class is represented in each fold

### 4. Model Building & Hyperparameter Tuning
- Train various machine learning models
- Apply sampling techniques (e.g., SMOTE, undersampling)
- Tune hyperparameters for optimal performance

### 5. Model Evaluation
- Use metrics suited for imbalanced data:
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
- Focus on minimizing false negatives (missed frauds)

---

## 📌 Notes

Due to GitHub's file size limit (100 MB), the dataset is not included in this repository. You can download it directly from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place it in your working directory.

---

## 👤 Contributor

**Shravan Madipelly**


