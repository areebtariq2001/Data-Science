# Task 4: Loan Default Risk with Business Cost Optimization

## Objective
Predict the likelihood of loan default and optimize the decision threshold based on 
a cost-benefit analysis, rather than relying on the default 0.5 classification threshold.

## Dataset
Home Credit Default Risk Dataset (Kaggle) — 307,511 loan applications with 
demographic, financial, and credit history features.

## Approach
- Cleaned the dataset by dropping columns with >40% missing values, imputing the rest
- Fixed a known anomaly in `DAYS_EMPLOYED` (placeholder value of 365243)
- Encoded categorical features and trained two classification models: Logistic 
  Regression and CatBoost, both with class balancing for the imbalanced target (~8% default rate)
- Defined business costs: False Negative (missed default) = $2500, False Positive 
  (rejected good customer) = $500
- Swept decision thresholds from 0.1 to 0.9 to find the cost-minimizing threshold
- Analyzed feature importance to identify key default risk drivers

## Results & Findings
- CatBoost outperformed Logistic Regression (ROC-AUC: 0.758 vs 0.744)
- **Optimal decision threshold: 0.69** (vs default 0.5), reducing total business 
  cost from ~$1.2M to ~$1.05M
- Top predictive features: external credit scores (EXT_SOURCE variables), age 
  (DAYS_BIRTH), and employment duration (DAYS_EMPLOYED)
- Demonstrates that aligning the decision threshold with actual business costs — 
  rather than using a generic 0.5 cutoff — significantly improves financial outcomes

## Files
- `Task4_Loan_Default.ipynb` — Full notebook with preprocessing, modeling, cost optimization, and feature importance
