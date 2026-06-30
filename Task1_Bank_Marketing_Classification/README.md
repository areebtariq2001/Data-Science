# Task 1: Term Deposit Subscription Prediction (Bank Marketing)

## Objective
Predict whether a bank customer will subscribe to a term deposit as a result of a 
marketing campaign, using classification models with explainable AI techniques.

## Dataset
Bank Marketing Dataset (UCI Machine Learning Repository) — 41,188 customer records 
with demographic, campaign, and economic context features.

## Approach
- Loaded and explored the dataset, analyzing the target distribution (imbalanced: 
  ~89% no, ~11% yes)
- Performed EDA on job, marital status, education, and age vs subscription outcome
- Encoded all categorical features using Label Encoding
- Trained two classification models: Logistic Regression and Random Forest, both 
  with class balancing to handle the imbalanced target
- Evaluated models using Confusion Matrix, F1-Score, and ROC Curve
- Used SHAP (TreeExplainer) to explain global feature importance and 5 individual 
  predictions via waterfall plots

## Results & Findings
- Random Forest outperformed Logistic Regression (higher F1-score and AUC), 
  effectively capturing non-linear relationships in customer behavior
- Key predictive features identified via SHAP: `duration`, `euribor3m`, 
  `nr.employed`, `age`, and `campaign`
- Customers with longer call durations and contacted during favorable economic 
  conditions (low euribor3m) showed higher subscription likelihood
- These insights can help the bank target high-probability customers, improving 
  campaign efficiency and reducing marketing cost

## Files
- `bank-additional-full.ipynb` — Full notebook with EDA, modeling, evaluation, and SHAP analysis
