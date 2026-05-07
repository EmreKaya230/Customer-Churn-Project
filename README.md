Project Overview

This project predicts customer churn for a telecommunications provider to identify at-risk users and support retention strategies. The dataset contains 7,043 customers with 20 features including contract type, monthly charges, and tenure.

Results

ModelAccuracyF1 (Churn)ROC-AUC
Logistic Regression=0.784, 0.427 ,0.829
Random Forest=0.790, 0.519, 0.822
XGBoost=0.779, 0.544, 0.812
XGBoost achieved the best F1 score for churn detection (0.544), making it the preferred model since correctly identifying churners is more important than overall accuracy.

Key Findings

Month-to-month contract customers churn at 43% vs 3% for two-year contracts
Churned customers pay on average $13 more per month ($74 vs $61)
Customers who churn have significantly lower tenure (18 months vs 38 months)

Technical Implementation

Data Cleaning: TotalCharges converted from string to numeric, 11 null rows dropped
Feature Engineering: One-hot encoding for categorical variables, StandardScaler for Logistic Regression
Models: Logistic Regression, Random Forest, XGBoost
Evaluation: Accuracy, F1-score, ROC-AUC, Confusion Matrix

Tech Stack

Python, Scikit-learn, XGBoost, Pandas, NumPy, Matplotlib
