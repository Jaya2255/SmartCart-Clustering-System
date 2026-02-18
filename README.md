# 🛒 SmartCart: Intelligent Customer Segmentation

**An Unsupervised Machine Learning solution to drive personalized marketing and customer retention for e-commerce.**

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)]()
[![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)]()
[![Status](https://img.shields.io/badge/Status-Completed-green)]()

---

## 📌 Problem Statement
**SmartCart**, a growing multi-national e-commerce platform, possesses extensive data on 2,240 customers. However, the company currently relies on **generic marketing strategies** for all users. 

This "one-size-fits-all" approach has led to three major business problems:
1. **Inefficient Marketing:** Wasted ad spend on the wrong demographics.
2. **Missed Opportunities:** Failure to identify and reward high-value, loyal customers.
3. **Customer Churn:** Delayed identification of users who are disengaged.

## 💡 The Solution
As an **AI/ML Engineer**, I developed an intelligent segmentation system using **Unsupervised Machine Learning**. Instead of predicting a specific outcome, this system analyzes historical transaction data, demographics, and website activity to discover hidden behavioral patterns.

The system automatically groups customers into **meaningful clusters**, allowing the marketing team to transition from generic campaigns to highly targeted, data-driven decisions.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (K-Means Clustering, Agglomerative Clustering, PCA)
* **Techniques:** Dimensionality Reduction, Elbow Method (KneeLocator), Silhouette Scoring, Feature Engineering, Feature Scaling

---

## 📊 Key Workflow

1. **Data Preprocessing & Feature Engineering:** * Imputed missing income values using median strategies.
   * Engineered high-value business features including `Age`, `Customer_Tenure_Days`, `Total_Spending`, and `Total_Children`.
   * Consolidated categorical variables (e.g., grouping Marital Status into `Living_With`).
   * Removed extreme outliers (Age > 90, Income > 600,000) to ensure model accuracy.
2. **Encoding & Scaling:** Applied `OneHotEncoder` for categorical variables and `StandardScaler` to normalize the data, a mandatory step for distance-based clustering.
3. **Dimensionality Reduction (PCA):** Applied Principal Component Analysis (PCA) to reduce the data down to 3 principal components, removing noise and enabling 3D visualization of the customer base.
4. **Clustering Optimization:** Mathematically determined the optimal number of clusters (k=4) by analyzing both the **Elbow Method** (via `Kneed`) and the **Silhouette Score**.
5. **Model Training:** Implemented and compared both **K-Means** and **Agglomerative (Hierarchical) Clustering** to segment the customer base.
6. **Cluster Profiling:** Analyzed the final 4 clusters by mapping Income vs. Total Spending, allowing the business to clearly define user personas (e.g., High-Income/High-Spenders vs. Low-Income/Low-Spenders).

---

## 📈 Business Outcome
By segmenting the customer base into 4 distinct groups, the marketing team can now deploy personalized offers to specific clusters. This optimizes campaign ROI, reduces marketing waste, and improves the retention of high-value customers.
