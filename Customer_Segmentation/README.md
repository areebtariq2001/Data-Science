# Task 2: Customer Segmentation Using Unsupervised Learning

## Objective
Cluster mall customers based on spending habits and propose marketing strategies 
tailored to each segment.

## Dataset
Mall Customers Dataset — 200 customer records with Age, Annual Income, and 
Spending Score.

## Approach
- Conducted EDA on age, income, and spending score distributions
- Applied K-Means Clustering, using the Elbow Method and Silhouette Score to 
  determine the optimal number of clusters (k=5, silhouette score ≈ 0.43)
- Visualized clusters using PCA and t-SNE for dimensionality reduction
- Profiled each cluster's average age, income, and spending score
- Proposed targeted marketing strategies for each segment

## Results & Findings
Five distinct customer segments were identified:
- **Cautious Seniors** (Age ~46, Income ~$27k, Spending ~18) — low income, low 
  spending older customers. Strategy: value-for-money deals, loyalty discounts.
- **Young Spenders** (Age ~25, Income ~$41k, Spending ~62) — largest segment (54 
  customers), young with moderate income but high spending. Strategy: trendy 
  products, social media campaigns, flexible payment options.
- **Premium Customers** (Age ~33, Income ~$86k, Spending ~82) — high income, high 
  spending, most valuable segment. Strategy: VIP loyalty programs, premium offerings.
- **Careful Affluent** (Age ~40, Income ~$86k, Spending ~19) — high income but low 
  spending, untapped potential. Strategy: targeted incentives to unlock spending.
- **Average Mainstream** (Age ~56, Income ~$54k, Spending ~49) — balanced segment 
  (47 customers). Strategy: standard seasonal promotions.

PCA and t-SNE visualizations confirmed clear separation between clusters, validating 
clustering quality.

## Files
- `Customer_Segmentation-Task2.ipynb` — Full notebook with EDA, clustering, visualization, and strategy recommendations
