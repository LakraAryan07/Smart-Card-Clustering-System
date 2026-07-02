# Smart Card Clustering System

# Smart Card Customer Segmentation Pipeline

An end-to-end unsupervised machine learning pipeline designed to preprocess, clean, and engineer raw transactional and demographic customer data[cite: 1]. By leveraging dimensionality reduction and advanced clustering techniques, this project segments "Smart Card" users into distinct, actionable behavioral profiles to optimize targeted marketing strategies[cite: 1].

---

## 📌 Project Overview
Understanding customer behavior is essential for building data-driven marketing campaigns. This repository takes raw CRM customer profiles and applies a rigorous data science workflow to segment customers based on demographic attributes, purchasing habits, and engagement history[cite: 1].

### Key Features Summary:
* **Data Cleaning & Imputation:** Systematically handles missing values and maps noisy categorical inputs into structural bins[cite: 1].
* **Feature Engineering:** Derives meaningful indicators such as absolute Customer Age, Total Spendings, Total Children, and Customer Tenure[cite: 1].
* **Dimensionality Reduction:** Utilizes Principal Component Analysis (PCA) to compress high-dimensional feature spaces[cite: 1].
* **Advanced Clustering:** Implements and compares K-Means Clustering (optimized via the Elbow Method/Silhouette Scores) and Agglomerative Hierarchical Clustering[cite: 1].

---

## 🛠️ Technology Stack
The pipeline is built purely in Python utilizing standard data science and machine learning libraries:
* **Data Manipulation:** `pandas`, `numpy`[cite: 1]
* **Data Visualization:** `matplotlib`, `seaborn`[cite: 1]
* **Machine Learning & Analytics:** `scikit-learn`[cite: 1]
* **Optimization:** `kneed` (KneeLocator for automated cluster selection)[cite: 1]

---

## 🚀 Pipeline Workflow

### 1. Data Processing & Cleansing
* Missing values within the `Income` variable are filled using robust median imputation[cite: 1].
* Highly correlated, redundant, or sparse categories are systematically dropped to prevent overfitting and multicollinearity[cite: 1].

### 2. Categorical Transformations
* **Education:** Re-mapped from five scattered degrees into three clean tiers: `UnderGraduate`, `Graduate`, and `PostGraduate`[cite: 1].
* **Marital Status:** Streamlined into simplified relationship statuses: `Partner` or `Alone`[cite: 1].

### 3. Scaling & Modeling (Upcoming)
* Features are encoded via **One-Hot Encoding** and standardized using **StandardScaler** to ensure uniform distance computations[cite: 1].
* **PCA** transforms the feature space into principal components to remove noise[cite: 1].
* **K-Means & Agglomerative Clustering** partition the user base into distinct marketing segments[cite: 1].

---

Summary

This project builds an end-to-end unsupervised machine learning pipeline that preprocesses, engineers, and cleans 
transactional/demographic customer data in order to segment "Smart Card" users using PCA and advanced clustering algorithms.
