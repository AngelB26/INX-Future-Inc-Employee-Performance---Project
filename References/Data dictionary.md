# 📊 Dataset Description - INX Future Inc Employee Performance

## 📁 Source
The dataset is sourced from INX Future Inc, a hypothetical corporate entity simulating real-world HR analytics data.

## 📦 Overview
The dataset comprises structured information on employees across departments and roles, including job satisfaction, performance indicators, and employment history.

## 📐 Shape and Size
- Total Records: 1,200 employees (approx.)
- Features: 20+

## 🧬 Key Features

| Feature Name                          | Description                                                    |
|--------------------------------------|----------------------------------------------------------------|
| EmpID                                | Unique employee identifier                                     |
| EmpLastSalaryHikePercent             | Percentage hike in last salary                                 |
| EmpEnvironmentSatisfaction           | Satisfaction with work environment (1–4 scale)                 |
| EmpWorkLifeBalance                   | Work-life balance rating (1–4 scale)                           |
| YearsSinceLastPromotion              | Years since last promotion                                     |
| ExperienceYearsInCurrentRole         | Experience in current role (in years)                          |
| YearsWithCurrManager                 | Years working with the current manager                         |
| EmpHourlyRate                        | Hourly wage of the employee                                    |
| EmpJobRole                           | Role of the employee (e.g., Developer, Manager)                |
| EmpDepartment                        | Department name (e.g., Sales, HR, Development)                 |
| EmpJobLevel                          | Level/grade of the job role                                    |
| BusinessTravelFrequency              | Frequency of business travel (Rarely, Frequently, etc.)        |
| MaritalStatus                        | Marital status (Single, Married, Divorced)                     |
| EducationBackground                  | Background in education (e.g., Technical, Other)               |
| PerformanceRating (Target Variable)  | Final performance class (0: Low, 1: Average, 2: High)          |

## 🎯 Target Variable
- `PerformanceRating`: A multiclass target representing employee performance levels:
  - **0**: Low Performer
  - **1**: Average Performer
  - **2**: High Performer

## ❗ Notes
- Missing values were handled via imputation.
- Categorical variables were encoded for modeling.
- The dataset mimics real corporate HR data for predictive analytics.

---

