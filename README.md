Customer Review Sentiment Analysis - Product Insights Report

Dataset
- Source: Amazon Fine Food Reviews
- Size: 20,000 reviews
- Ratings: 1-5 stars

Sentiment Distribution
- Positive (4-5 stars): 15,595 reviews (78%)
- Negative (1-2 stars): 2,886 reviews (14%)
- Neutral (3 stars): 1,519 reviews (8%)

Model Performance
- TF-IDF + Logistic Regression: Accuracy 76%, F1 0.87 (positive), F1 0.59 (negative)
- DistilBERT zero-shot: Accuracy 62%, F1 0.72 (positive), F1 0.44 (negative)
- TF-IDF model outperforms DistilBERT zero-shot on this domain-specific dataset

Top Complaints from Negative Reviews
1. Poor Taste & Flavor - customers unhappy with taste, texture, and flavor
2. Fake & Wasteful Products - chocolate, cocoa products labeled as fake or misleading
3. Coffee & Tea Quality - bitter taste, poor roast quality
4. Shipping & Packaging - damaged boxes, wrong items, Amazon delivery issues
5. Food Origin Concerns - products made in China, dog food quality issues
6. Specific Product Issues - jerky, olive oil, cherry products frequently complained about

Top Praise Themes from Positive Reviews
- Great taste and flavor
- Good value for money
- Fresh and high quality ingredients
- Fast delivery and good packaging

3 Actionable Recommendations
1. Improve product labeling - customers feel misled about ingredients and origin
2. Review chocolate and cocoa product quality - high complaint volume in this category
3. Strengthen packaging for shipping - many complaints about damaged or wrong items

How to Run
1. Clone the repository
2. Install: pip install -r requirements.txt
3. Place Reviews.csv in project folder
4. Open sentiment_analysis.ipynb and run all cells
