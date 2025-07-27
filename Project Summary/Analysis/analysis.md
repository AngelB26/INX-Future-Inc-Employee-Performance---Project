# 📊 Employee Performance Analysis - Exploratory and Model Evaluation Report

## 1. Project Objective
The primary goal of this project is to predict employee performance (Low, Average, High) based on various demographic, professional, and behavioral features using machine learning models. The outcome can help HR departments in decision-making regarding hiring, promotion, and training.

---

## 2. Data Overview

- **Initial Dataset Size:** 768 records
- **Target Classes:** 3 (0 = Low, 1 = Average, 2 = High performers)
- **No. of Features after Preprocessing:** 30+
- **No. of Final Selected Features for Modeling:** 20

---

## 3. Data Cleaning & Preprocessing

- ✔️ **Missing Values:** Handled (all cleaned)
- ✔️ **Encoding:** One-Hot Encoding for categorical variables
- ✔️ **Outlier Treatment:** IQR and Median Capping
- ✔️ **Scaling:** RobustScaler applied on numerical features
- ✔️ **Train-Test Split:** 70-30 ratio
  - Training: 528 samples
  - Testing: 240 samples

---

## 4. Feature Engineering & Selection

- 🔍 Applied **Mutual Information** and **F-score** methods for feature importance ranking
- ✅ **Top Features Identified:**
  - EmpLastSalaryHikePercent
  - EmpEnvironmentSatisfaction
  - YearsSinceLastPromotion
  - ExperienceYearsInCurrentRole
  - EmpWorkLifeBalance

- 📉 Final features scaled using RobustScaler

---

## 5. Model Training & Evaluation

**Trained Models:**
1. Logistic Regression
2. K-Nearest Neighbors
3. Naive Bayes
4. Support Vector Machine
5. Decision Tree
6. Random Forest
7. XGBoost
8. Gradient Boosting

**Best Model:** ✅ Gradient Boosting  
**Best Accuracy:** `93.33%`

---

## 6. Gradient Boosting Model Insights

- **Top Features by Importance:**
  - EmpEnvironmentSatisfaction (28.3%)
  - EmpLastSalaryHikePercent (25.7%)
  - YearsSinceLastPromotion (20.4%)

- **Performance Metrics:**
  - Precision: 0.93
  - Recall: 0.93
  - F1-Score: 0.93

- ⚠️ High performers (Class 2) showed a slightly lower recall (0.77)

---

## 7. Visualizations

- Confusion Matrix
- Top 15 Features Plot
- Correlation Heatmap
- Distribution Plots for Key Variables

---

## 8. Conclusion

Gradient Boosting performed the best and is deployed as the final model. Feature importance insights can drive policy and hiring improvements. Regular retraining and validation are recommended for continued performance.


