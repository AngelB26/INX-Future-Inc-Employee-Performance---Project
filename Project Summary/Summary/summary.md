
---

### ✅ `summary.md`

```markdown
# 🧾 Final Project Summary – Employee Performance Analysis

## 🎯 Objective
To classify employee performance into 3 levels (Low, Average, High) using historical HR and performance data, assisting decision-makers in promotions, training, and retention.

---

## 🗃️ Dataset Summary

- Records: 768
- Target Classes: 3
- Features used for modeling: 20

---

## 🛠️ Approach

1. **Data Cleaning**
   - Handled missing values and outliers
2. **Feature Engineering**
   - One-Hot Encoding
   - Feature Scaling (RobustScaler)
   - Mutual Information + F-score for selection
3. **Model Training**
   - Evaluated 8 classification models
4. **Model Selection**
   - Best Model: ✅ Gradient Boosting
   - Accuracy: 93.33%

---

## 📌 Key Results

- **Top Features:**
  - EmpEnvironmentSatisfaction
  - EmpLastSalaryHikePercent
  - YearsSinceLastPromotion

- **Model Evaluation:**
  - Accuracy: 93%
  - High recall for average performers
  - Moderate recall for high performers (⚠️ room for improvement)

---

## 📦 Outputs

- Saved Model: `best_model.pkl`
- Feature Importance: `feature_importance.csv`
- Model Results Summary: `model_results.csv`

---

## 🚀 Recommendations

- Deploy the Gradient Boosting model for real-time employee performance prediction
- Review low recall in high performers – consider resampling or feature expansion
- Perform monthly retraining with updated data

---

## 📍 Conclusion

This analysis provides actionable insights and a robust model for employee performance classification. It lays the groundwork for smarter HR decisions driven by data.

