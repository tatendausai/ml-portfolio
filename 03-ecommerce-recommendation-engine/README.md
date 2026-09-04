# Amazon Electronics Recommendation Engine

## Overview
Multi-model recommendation system built on Amazon product reviews, filtering high-activity users (≥50 ratings) and high-demand products (≥5 ratings) to address e-commerce catalog sparsity.

## Key Findings
* **User-User Collaborative Filtering:** Optimized `KNNBasic` with Cosine similarity outperformed Item-Item and Matrix Factorization models, reaching an **F1@10 score of 87.1%** and a **Recall@10 of 89.9%**.
* **Matrix Factorization:** `SVD` achieved the lowest rating prediction error (**RMSE: 0.8977**) after tuning the learning rate and regularization, with a comparable ranking relevance score (**F1: 86.8%**).

## Recommendations
* Deploy tuned user-user collaborative filtering for personalized homepage recommendations.
* Explore a hybrid architecture combining SVD latent factors with neighborhood user similarity to mitigate cold-start issues.

## Tech Stack
* **Language & Libraries:** Python, Scikit-Surprise, Scikit-Learn, Pandas, NumPy
