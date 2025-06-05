# Project-Rene Winds: Predictive Modeling with Ensemble Learning
**Overview**

This project applies various ensemble learning methods (including Random Forest, AdaBoost, Bagging, and Gradient Boosting) to a classification problem with class imbalance. The goal is to accurately predict the target class while addressing data imbalance using SMOTE oversampling and Random UnderSampling techniques.

**Techniques Used**
- Exploratory Data Analysis (EDA):Exploratory Data Analysis (EDA) is a crucial first step in data analysis, allowing us to understand the dataset's structure, detect anomalies, and uncover underlying patterns. In this project, EDA was performed to assess data quality and inform subsequent modeling decisions.

- Missing Value Imputation using SimpleImputer:To ensure consistency and handle missing data effectively,used SimpleImputer from Scikit-learn with the median strategy.

- Feature Scaling using StandardScaler:After imputing missing values,applied feature scaling using StandardScaler from Scikit-learn to normalize the data.

- Handling Class Imbalance:The dataset was highly imbalanced, with significantly fewer positive class instances. To address this,applied both oversampling and undersampling strategies:
  - Oversampling: SMOTE- used SMOTE (Synthetic Minority Over-sampling Technique) to synthetically generate new samples for the minority class.
    
    - before oversampling,count of class 0:  14167
    - before oversampling,count of class 1:  833
    - after oversampling,count of class 0:  14167
    - after oversampling,count of class 1:  14167
  - Undersampling: RandomUnderSampler-also experimented with RandomUnderSampler to reduce the number of majority class samples.
    
      - before undersampling,count of class 0:  14167
      - before undersampling,count of class 1:  833
      - after undersampling,count of class 0:  833
      - after undersampling,count of class 1:  833
 
- Feature Importance:To understand which features contributed most to the final model’s predictions,extracted feature importances from the best-performing AdaBoost Classifier

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


