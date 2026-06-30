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
- **Cautious Seniors** (low income, low spending) — value-focused offers
- **Young Spenders** (low-mid income, high spending) — trend-driven, social media marketing
- **Premium Customers** (high income, high spending) — VIP loyalty programs
- **Careful Affluent** (high income, low spending) — targeted incentives to unlock potential
- **Average Mainstream** (mid income, mid spending) — standard seasonal promotions

PCA and t-SNE visualizations confirmed clear separation between clusters, validating 
clustering quality.

## Files
- `Task2_Customer_Segmentation.ipynb` — Full notebook with EDA, clustering, visualization, and strategy recommendations
