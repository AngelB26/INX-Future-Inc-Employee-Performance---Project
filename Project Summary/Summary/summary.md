# Final Project Summary – Employee Performance Analysis

## 🎯 Objective

To classify employee performance into three levels (Low, Average, High) using historical HR and performance data, aiding in decisions related to promotions, training, and retention.

---

## 🗃️ Dataset Summary

- **Total Records**: 768
- **Target Classes**: 3 (Low, Average, High)
- **Features Used**: 20

---

## 🛠️ Approach

1. **Data Cleaning**
   - Handled missing values and outliers

2. **Feature Engineering**
   - One-Hot Encoding
   - Feature Scaling using RobustScaler
   - Feature selection using Mutual Information and F-score

3. **Model Training**
   - Evaluated 8 classification models

4. **Model Selection**
   - **Best Model**: Gradient Boosting
   - **Accuracy**: 93.33%

---

## 📌 Key Results

- **Top Features**:
  - EmpEnvironmentSatisfaction
  - EmpLastSalaryHikePercent
  - YearsSinceLastPromotion

- **Evaluation Metrics**:
  - **Overall Accuracy**: 93%
  - High recall for average performers
  - Moderate recall for high performers *(room for improvement)*

---

## 📦 Output Files

- `best_model.pkl` – Final trained model
- `feature_importance.csv` – Ranked feature importances
- `model_results.csv` – Metrics for all evaluated models

---

## 🚀 Recommendations

- Deploy the Gradient Boosting model for real-time predictions
- Improve high performer recall via resampling or advanced features
- Retrain model monthly using updated performance records

---

## 📍 Conclusion

This project delivers a high-performing model to classify employee performance and provides actionable insights for HR strategy. With periodic retraining, it can remain robust and relevant in dynamic organizational environments.
