# Bank Customer Churn Prediction: From Linear to Ensemble Learning

This project aims to predict bank customer churn (attrition) using machine learning techniques. I explored the transition from a baseline linear model to a complex ensemble model to maximize the recall rate for identifying customers at risk.

##  Project Overview
Predicting churn is vital for banks to retain their high-value customers. In this study:
- **Dataset:** 10,000 customer records including demographics and financial status.
- **Problem:** Binary Classification (Stay vs. Exit).
- **Goal:** Improve the identification of customers who are actually leaving (High Recall).

##  Model Evolution & Comparison

I followed an iterative approach to find the most effective solution:

### Phase 1: Baseline Model (Logistic Regression)
Started with a simple linear approach to establish a baseline.
- **Accuracy:** ~81%
- **Recall (Target Class):** ~20%
- **Analysis:** While the overall accuracy was decent, the model failed to capture the majority of customers who were actually leaving. The relationship in the data was too complex for a linear boundary.

### Phase 2: Advanced Model (Random Forest)
Implemented a **Random Forest Classifier** with 100 decision trees to capture non-linear patterns.
- **Accuracy:** **~86%**
- **Recall (Target Class):** **~46%**
- **Result:** Switching to an ensemble method resulted in a **130% improvement** in detecting churned customers.

##  Key Insights (Feature Importance)
The model revealed that the most critical factors influencing a customer's decision to leave are:
1. **Age:** Older customers showed a higher tendency to churn.
2. **Estimated Salary & Balance:** Financial stability plays a significant role in loyalty.
3. **IsActiveMember:** Active engagement is the strongest deterrent against churn.

##  Tech Stack & Skills
- **Python / Jupyter Notebook**
- **Pandas & NumPy:** For data preprocessing and "One-Hot Encoding" for geographical data.
- **Scikit-Learn:** For model training, evaluation metrics, and `train_test_split`.
- **Seaborn & Matplotlib:** For visualizing the Confusion Matrix and Feature Importance.
