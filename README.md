E-Commerce Recommendation Engine 🚀

Overview

This project focuses on building a smarter, data-driven recommendation engine for an e-commerce website. The current recommendation system relies on most popular items, lacking personalization and losing revenue potential. Our solution applies K-Means clustering to segment customers based on their buying behavior and generate tailored product recommendations.

🔑 Key Features

Customer Segmentation using K-Means

Personalized Recommendations for Each Cluster

Discount Offer Optimization based on Recency & Frequency

Expected Monetary Value Calculation for Model Evaluation

Performance Comparison Against the Base Model

🔬 Methodology

1. Why K-Means?

We evaluated multiple clustering algorithms and selected K-Means based on:

Performance: Best balance of accuracy & efficiency for large datasets.

Interpretability: Provides clear customer segmentation.

Scalability: Computationally efficient compared to hierarchical models.

2. Data Preprocessing & Feature Engineering

Extracted key customer metrics:

Recency (R): How recently a customer made a purchase.

Frequency (F): How often they purchase.

Monetary Value (M): Total spending amount.

Standardized data using MinMax Scaler for better clustering performance.

Applied Principal Component Analysis (PCA) to reduce dimensionality while retaining 76% variance.

3. Clustering Evaluation Metrics

To ensure high-quality clustering, we optimized K-Means using:

Silhouette Score: 0.30 (higher is better)

Davies-Bouldin Index (DBI): 1.34 (lower is better)

Variance Ratio Criterion (VRC): 5100.74 (higher is better)

4. Model Optimization Strategy

Feature Selection: Focused on relevant behavioral metrics.

Outlier Removal: Used z-score filtering (z > 3) to eliminate anomalies.

Hyperparameter Tuning: Tested 220 combinations of k-values, PCA components, and additional features to maximize clustering performance.

📈 Key Findings & Model Performance

Distinct Customer Segments Identified: Customers grouped based on purchase patterns.

Optimized Discount Strategy:

30% discount for high-value, low-frequency customers (Q4 Recency, Q1 Frequency)

15% discount for moderately engaged customers (Q3 Recency, Q2 Frequency)

Monetary Value Prediction:

Base Model Total: 817

Cluster Model Total: 3042

272% improvement in expected revenue.

🛠️ Technical Stack

Python: Core programming language

Libraries Used:

Scikit-learn: K-Means clustering, PCA

NumPy & Pandas: Data processing

Matplotlib & Seaborn: Data visualization

Scipy: Outlier detection

🎯 Business Impact

Personalized Recommendations: Higher engagement and conversion rates.

Revenue Boost: Better targeting of customer preferences.

Data-Driven Decision Making: Optimized pricing and discount strategies.

🚀 Future Enhancements

Hybrid Model: Combine collaborative filtering with K-Means for more robust recommendations.

Deep Learning Integration: Leverage Neural Networks (Autoencoders) for feature extraction.

Real-Time Personalization: Deploy real-time recommendation engine based on session activity.

Authors: Danylo Sovgut, Ke Wang, Shane Kim, Chris Korabik, Dean Q, Nathan Bywood, Vicki Yuan.

