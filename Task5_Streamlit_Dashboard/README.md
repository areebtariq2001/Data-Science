# Task 5: Interactive Business Dashboard in Streamlit

## Objective
Develop an interactive dashboard for analyzing sales, profit, and segment-wise 
performance of a global retail business.

## Dataset
Global Superstore Dataset (Sample - Superstore.csv) — order-level sales, profit, 
and customer data across regions, categories, and sub-categories.

## Approach
- Cleaned and prepared the dataset for dashboard consumption
- Built an interactive Streamlit dashboard with sidebar filters for Region, 
  Category, and Sub-Category
- Displayed key KPIs: Total Sales, Total Profit, Total Orders, Profit Margin
- Created visualizations using Plotly: Sales by Category, Profit by Category, 
  Sales Trend Over Time, Sales by Region, Top 5 Customers by Sales, and a 
  Sub-Category Performance table

## How to Run
```bash
pip install streamlit plotly pandas
streamlit run dashboard.py
```
Ensure `Sample - Superstore.csv` is in the same directory as `dashboard.py`.

## Results & Findings
The dashboard enables dynamic, filter-driven exploration of business performance, 
allowing stakeholders to quickly identify top-performing regions, categories, and 
customers. Interactive KPIs and charts support faster, data-driven decision making 
compared to static reports.

## Files
- `dashboard.py` — Streamlit dashboard application
