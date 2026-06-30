# Data Science Internship — Advanced Tasks
### DevelopersHub Corporation

This repository contains 5 advanced data science tasks completed as part of my 
Data Science Internship at DevelopersHub Corporation. Each task tackles a real-world 
problem using industry-standard tools and libraries including pandas, scikit-learn, 
XGBoost, CatBoost, SHAP, Prophet, and Streamlit.

## Tasks Overview

| # | Task | Domain | Key Techniques |
|---|------|--------|-----------------|
| 1 | [Bank Marketing Classification](./Task1_Bank_Marketing_Classification) | Classification | Logistic Regression, Random Forest, SHAP |
| 2 | [Customer Segmentation](./Customer_Segmentation) | Unsupervised Learning | K-Means, PCA, t-SNE |
| 3 | [Energy Consumption Forecasting](./Energy_Forecasting) | Time Series | ARIMA, Prophet, XGBoost |
| 4 | [Loan Default Risk](./Loan_Default_Risk) | Classification + Cost Optimization | Logistic Regression, CatBoost, Threshold Tuning |
| 5 | [Business Intelligence Dashboard](./Task5_Streamlit_Dashboard) | BI / Dashboarding | Streamlit, Plotly |

## Task Summaries

**Task 1 — Bank Marketing Classification**
Predicted term deposit subscription using Logistic Regression and Random Forest, 
with SHAP-based explainability for 5 individual predictions. Random Forest achieved 
better F1-score and ROC-AUC, identifying `duration`, `euribor3m`, and `age` as top features.

**Task 2 — Customer Segmentation**
Segmented mall customers into 5 distinct groups using K-Means clustering (validated 
via Elbow Method and Silhouette Score), visualized with PCA and t-SNE, and proposed 
tailored marketing strategies for each segment.

**Task 3 — Energy Consumption Forecasting**
Forecasted hourly household power consumption by comparing ARIMA, Prophet, and 
XGBoost. Prophet achieved the best performance (MAE: 0.506, RMSE: 0.686) by 
capturing daily and weekly seasonality.

**Task 4 — Loan Default Risk**
Built a loan default classifier using Logistic Regression and CatBoost, then 
optimized the decision threshold (0.69 vs default 0.5) based on defined business 
costs, reducing total expected cost from ~$1.2M to ~$1.05M.

**Task 5 — Business Intelligence Dashboard**
Developed an interactive Streamlit dashboard for the Global Superstore dataset, 
featuring dynamic filters (Region, Category, Sub-Category), KPI cards, and 
visualizations for sales, profit, and top customers.

## Tools & Libraries Used
pandas, numpy, scikit-learn, xgboost, catboost, shap, prophet, statsmodels, 
matplotlib, seaborn, plotly, streamlit

## Author
Areeb Tariq
