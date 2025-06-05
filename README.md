# Project-Rene Winds: Predictive Modeling with Ensemble Learning
**Overview**

This project applies various ensemble learning methods (including Random Forest, AdaBoost, Bagging, and Gradient Boosting) to a classification problem with class imbalance. The goal is to accurately predict the target class while addressing data imbalance using SMOTE oversampling and Random UnderSampling techniques.

**Techniques Used**
- Exploratory Data Analysis (EDA)

- Missing Value Imputation using SimpleImputer

- Feature Scaling using StandardScaler

- Handling Class Imbalance
  - Oversampling: SMOTE
  - Undersampling: RandomUnderSampler
 
- Feature Importance

**Ensemble Learning Models:**

- Random Forest

- AdaBoost

- Gradient Boosting

- Bagging Classifier

- Logistic Regression (baseline)

- Decision Tree

**Model Evaluation**

- Accuracy, Recall, Precision, F1 Score

- Confusion Matrix

**Hyperparameter Tuning using RandomizedSearchCV**

Pipeline Integration with Pipeline

**Data Summary:**
- Total Features: 40

- Target Variable: Binary Classification (0/1)

- Train Size: 20,000 samples

- Test Size: 5,000 samples

- Class imbalance detected: Before oversampling: 14167 (class 0), 833 (class 1)

Final Selected Model: AdaBoost (Undersampled)-accuracy-0.9376%


