# 🏦 Loan Default Prediction Model

## 📌 Overview
This project focuses on building a machine learning pipeline to predict loan default risk using the Lending Club Loan Dataset. It includes comprehensive EDA, data preprocessing with SMOTE to handle class imbalance, model training with LightGBM and SVM, and detailed evaluation metrics including F1-score and ROC-AUC.

---

## 📁 Dataset

- **Source**: [Lending Club Loan Dataset (2007–2018) on Kaggle](https://www.kaggle.com/datasets/wordsforthewise/lending-club)
- Features include applicant financial details, loan amounts, interest rates, DTI, and repayment status.

---

## ⚙️ Pipeline Steps

1. **Exploratory Data Analysis (EDA)**  
   - Visualize missing values, distributions, and correlations.
   - Examine loan status distribution and default rate.

2. **Preprocessing & Feature Engineering**  
   - Remove unnecessary columns.
   - Encode categorical variables.
   - Scale numeric features using StandardScaler.
   - Handle class imbalance using SMOTE.

3. **Model Training**  
   - Train LightGBM and SVM classifiers.
   - Tune and compare models.

4. **Evaluation Metrics**  
   - Precision, Recall, F1-Score.
   - ROC Curve & AUC Score.
   - Feature Importance analysis.

---

## 📊 Results

- LightGBM outperforms SVM in recall and AUC, making it more suitable for identifying high-risk applicants.
- Key features include: interest rate, debt-to-income ratio, and revolving balance.

---

## 🧠 Recommendations

- Cap interest rates for high DTI customers.
- Use high-recall models for early filtering and high-precision ones for final screening.
- Update models periodically to adapt to new lending trends.

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/loan-default-prediction-model.git
   cd loan-default-prediction-model
