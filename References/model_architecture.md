# 🧠 Model Architecture – Employee Performance Prediction

This document outlines the architecture used for building the **Employee Performance Prediction Model** for **INX Future Inc**.

---

## 📁 1. Data Ingestion

- Load employee dataset from CSV/Excel files.
- Perform basic inspections using `.head()`, `.info()`, `.describe()`.

---

## 🧹 2. Data Cleaning

- Drop irrelevant columns (e.g., `EmployeeID`).
- Handle missing values:
  - Numerical: Imputed using **median**.
  - Categorical: Imputed using **mode**.
- Remove duplicate entries if any.

---

## 🔍 3. Exploratory Data Analysis (EDA)

- Analyze distributions of key variables.
- Visualizations:
  - **Distribution plots** for continuous features.
  - **Count plots** for categorical features.
  - **Boxplots** for outlier detection.
  - **Heatmap** for feature correlation.
- Identify class imbalances and potential data leakage.

---

## 🏗️ 4. Feature Engineering

- Encode categorical variables:
  - Label Encoding for target (`PerformanceRating`)
  - One-Hot Encoding or Label Encoding for features
- Create new features if relevant (e.g., experience buckets)
- Feature scaling using **RobustScaler**

---

## 📤 5. Data Splitting

- Split data into **train** and **test** sets using stratified sampling.
- Typical split: **80% training**, **20% testing**.

---

## 🤖 6. Model Training

Trained multiple classification models:
- **Random Forest**
- **XGBoost**
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Decision Tree**
- **K-Nearest Neighbors (KNN)**
- **Gradient Boosting**
- **Naive Bayes**

---

## 🔎 7. Model Evaluation

- Metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Cross-Validation Scores

- Identified Top 3 Models:
  1. Gradient Boosting
  2. Random Forest
  3. XGBoost

---

## 🛠️ 8. Hyperparameter Tuning

- Performed GridSearchCV for top models
- Tuned parameters like:
  - `learning_rate`, `n_estimators`, `max_depth` (for Gradient Boosting)
- Selected best model based on validation score

---

## 📊 9. Feature Importance Analysis

- Extracted and visualized feature importances using the best tree-based model.
- Top contributing features were:
  - `EmpLastSalaryHikePercent`
  - `EmpEnvironmentSatisfaction`
  - `YearsSinceLastPromotion`

---

## 🧾 10. Results Summary

- **Best Model**: Gradient Boosting Classifier
- **Test Accuracy**: 93.75%
- Detailed metrics available in [summary.md](../summary.md)

---

## 📦 11. Model Saving

- Best model saved using `joblib`
- Ready for deployment and inference

---

## 📁 Folder Structure

