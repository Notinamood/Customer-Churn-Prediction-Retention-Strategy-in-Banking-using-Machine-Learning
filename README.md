# Customer Churn Prediction and Retention Strategy using Machine Learning

## Project Overview

This project focuses on predicting customer churn in the banking sector using machine learning techniques and deriving actionable business insights to reduce churn. The objective is not only to build accurate predictive models but also to understand the key factors driving churn and recommend effective retention strategies.

---

## Problem Statement

Customer churn is a critical issue for businesses as it directly impacts revenue and growth. Identifying customers who are likely to leave allows organizations to take proactive measures to retain them.

The goals of this project are:

* Predict whether a customer will churn
* Identify key factors influencing churn
* Provide data-driven recommendations to improve retention

---

## Dataset

The dataset consists of 10,000 banking customers and includes:

* Demographic information (Age, Gender, Geography)
* Financial attributes (Balance, Credit Score, Estimated Salary)
* Customer behavior (Number of Products, Activity status, Loyalty points)

---

## Methodology

### Data Preprocessing

* Removed irrelevant columns such as CustomerId and Surname
* Standardized column names
* Encoded categorical variables using one-hot encoding
* Verified data quality (no missing values, correct data types)

---

### Model Development

Two models were implemented:

1. Logistic Regression (baseline model)
2. Random Forest (improved model)

---

### Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Special focus was given to recall, as identifying churn customers is critical for business impact.

---

### Data Leakage Handling

Features such as `complain` and `satisfaction_score` were removed to prevent data leakage and ensure realistic model performance.

---

### Threshold Tuning

The classification threshold was adjusted from 0.5 to 0.45 to improve recall while maintaining acceptable precision, achieving a better balance between detecting churn and minimizing false positives.

---

## Results

### Logistic Regression

* High recall
* Low precision
* Suitable for identifying most churn customers but with many false positives

### Random Forest

* Accuracy: approximately 86%
* Precision: approximately 72%
* Recall: approximately 52% after threshold tuning

The Random Forest model provided a more balanced and realistic performance.

---
## Dasboard
![Dashboard](Customer Churn Prediction & Retention Strategy in Banking using Machine Learning/Visuals/Final20%_20%Visual20%.jpg)
## Key Insights

* Age is the most influential factor in predicting churn
* Customers with fewer products are more likely to churn
* Low balance customers show higher churn probability
* Customer engagement (loyalty points) plays a significant role in retention

---

## Business Recommendations

* Target customers with low product usage for cross-selling opportunities
* Enhance loyalty programs to increase engagement
* Focus on high-risk customers identified by the model
* Provide personalized offers based on customer segmentation

---

## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
---

## Conclusion

This project demonstrates a complete data science workflow, from data preprocessing to model development and business insight generation. It highlights the importance of balancing model performance metrics and translating technical results into actionable business strategies.
