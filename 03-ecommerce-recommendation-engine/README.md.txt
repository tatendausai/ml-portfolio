Amazon Electronics Recommendation Engine Overview: 

Multi-model recommendation system built on Amazon product reviews, filtering high-activity users ($\ge 50$ ratings) and high-demand products ($\ge 5$ ratings) to address e-commerce catalog sparsity.  

Key Findings:User-User Collaborative Filtering (KNNBasic with Cosine similarity) outperformed Item-Item and Matrix Factorization models after tuning, reaching an F1@10 score of 87.1% and a Recall@10 of 89.9%.  

Matrix Factorization (SVD) achieved the lowest prediction error (RMSE: 0.8977) after tuning learning rate and regularization, but scored slightly lower on ranking relevance (F1: 86.8%).  

Recommendations: Deploy tuned user-user collaborative filtering for personalized homepage recommendations, and explore a hybrid architecture combining SVD latent factors with user similarity for cold-start mitigations.  

Stack: Python, Scikit-Surprise, Scikit-Learn, Pandas, NumPy.  