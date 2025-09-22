# customer-segmentation

Customer Segmentation with K-Means
This project builds a production-ready customer segmentation system using K-Means clustering on transactional and demographic data. It includes a reproducible training pipeline, an inference API, optional Streamlit UI, experiment tracking, containerization, and CI/CD hooks for reliable deployment.

Objectives
Discover actionable customer segments from spending, engagement, and recency behaviors.

Expose a simple prediction service that assigns a new customer to a segment.

Ensure the pipeline is reproducible, testable, and deployable with standard MLOps practices.

Dataset
File: customer_segmentation.csv

Typical columns: demographics (Year_Birth, Education, Marital_Status), economics (Income), behavior (Recency, NumWebPurchases, NumStorePurchases, NumWebVisitsMonth), and category spend (MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts).

Derived features used for clustering:

Age = 2025 - Year_Birth

Total_Spending = sum of category spend columns

Final feature vector: [Age, Income, Total_Spending, NumWebPurchases, NumStorePurchases, NumWebVisitsMonth, Recency]

Features and Labels
Unsupervised clustering with K-Means; no labels in the raw data.

Optional human-readable segment names can be mapped post hoc for business reporting.
