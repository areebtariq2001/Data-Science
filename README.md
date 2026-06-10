Sales Demand Forecasting - Rossmann Store Sales

Objective
Forecast future retail sales using time series and machine learning on Rossmann Store Sales dataset.

Dataset
- Source: Kaggle - Rossmann Store Sales Competition
- Size: 1,017,209 rows, 9 features
- Stores used: 2, 3, 20, 30
- Date range: 2013-01-02 to 2015-07-31

Feature Engineering
- Year, Month, Day, WeekOfYear extracted from Date
- IsWeekend flag created from DayOfWeek
- Lag_7, Lag_14: sales 7 and 14 days ago
- Rolling_Mean_7, Rolling_Mean_14: rolling average sales
- Time-based train/test split used - no random shuffle

Models
- Prophet (classical time series model)
- LightGBM (tree-based model with lag features)

Results - Store 2
Model      | MAE     | RMSE    | MAPE
Prophet    | 1438.71 | 1814.58 | 32.26%
LightGBM   | 399.84  | 528.45  | 8.03%

Key Findings
- LightGBM outperforms Prophet significantly
- Lag features and rolling means are most important predictors
- Weekly seasonality is strong across all stores
- Store 2 is easiest to predict due to consistent patterns

How to Run
1. Clone the repository
2. Install dependencies: pip install -r requirements.txt
3. Place train.csv and store.csv in the project folder
4. Open sales_forecasting.ipynb in Jupyter Notebook
5. Run all cells in order
