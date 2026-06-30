# Task 3: Energy Consumption Time Series Forecasting

## Objective
Forecast short-term household energy usage using historical time-based patterns.

## Dataset
Household Power Consumption Dataset (UCI) — minute-level power consumption data 
over ~4 years, resampled to hourly granularity for modeling.

## Approach
- Parsed and resampled minute-level data to hourly averages (~35,000 rows)
- Engineered time-based features: hour of day, day, month, day of week, weekend flag
- Compared three forecasting models: ARIMA, Prophet, and XGBoost
- Evaluated models using MAE and RMSE on a 7-day holdout test period
- Visualized actual vs forecasted energy usage for each model

## Results & Findings
| Model | MAE | RMSE |
|-------|-----|------|
| ARIMA | 0.693 | 0.856 |
| **Prophet** | **0.506** | **0.686** |
| XGBoost | 0.516 | 0.708 |

- Prophet performed best, effectively capturing daily and weekly seasonality
- XGBoost performed comparably well using engineered time features
- ARIMA underperformed due to its limited ability to capture complex seasonality 
  without manual tuning
- Energy usage shows clear peaks during morning and evening hours, with distinct 
  weekday vs weekend patterns

## Files
- `Task3_Energy_Forecasting.ipynb` — Full notebook with feature engineering, model comparison, and forecasting visualizations
