# INX-Future-Inc-Employee-Performance---Project
## 📊 Employee Performance Analysis

A Machine Learning-based classification system to predict and categorize employee performance into **Low**, **Average**, and **High** levels. This helps HR departments make informed decisions on **promotions**, **training**, and **retention** strategies.

---

## 🎯 Objective

- Predict employee performance levels using historical HR and performance data.
- Assist organizations in identifying high-potential employees and those needing support.

---

## 🗃️ Dataset Summary

- **Total Records:** 768 employees  
- **Target Classes:**  
  - 0 → Low Performance  
  - 1 → Average Performance  
  - 2 → High Performance
- **Features:**  
  - Employee demographics  
  - Work experience  
  - Education  
  - Job role and tenure  
  - Evaluation metrics

---

## 🛠️ Tools & Technologies

- **Languages:** Python
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, xgboost
- **Modeling:** Gradient Boosting, Random Forest, XGBoost, SVM, Logistic Regression
- **IDE:** VS Code / Jupyter Notebook
- **Version Control:** Git & GitHub

---

## 🔄 Project Flowchart

```mermaid
flowchart TD
    A([Start]) --> B([Load Dataset])
    B --> C([Data Cleaning & Preprocessing])
    C --> D([Exploratory Data Analysis])
    D --> E([Feature Engineering])
    E --> F([Model Training & Evaluation])
    F --> G{Is Accuracy Satisfactory?}
    G -- No --> E
    G -- Yes --> H([Select Best Model: Gradient Boosting])
    H --> I([Model Interpretation<br>Classification Report])
    I --> J([Save Model & Results])
    J --> K([Generate Summary Reports])
    K --> L([End / Deployment Ready])
