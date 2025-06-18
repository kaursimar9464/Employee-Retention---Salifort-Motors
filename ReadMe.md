# Employee Turnover Prediction – Salifort Motors

This project, completed as part of the **Google Advanced Data Analytics Capstone**, analyzes HR data from Salifort Motors to identify key factors contributing to employee turnover. The goal is to help the organization reduce attrition by using predictive modeling and data-driven recommendations.

---

## Project Overview
- **Business Problem**: High employee turnover is costly and disruptive. The company seeks to understand why employees leave and how to improve retention.
- **Objective**: Predict whether an employee will leave based on factors like satisfaction, department, workload, and salary.
- **Dataset**: 15,000+ employee records with variables including satisfaction level, number of projects, average monthly hours, time at company, salary, and more. ([Kaggle dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv))

---

## Tools and Libraries
- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

---

## Model Summary
Three models were trained and evaluated:

| Model                | F1 Score | Accuracy | Recall   | Precision |
|---------------------|----------|----------|----------|-----------|
| Logistic Regression | 0.018    | 0.744    | 0.0098   | 0.103     |
| Random Forest       | 0.962    | 0.982    | 0.952    | 0.971     |
| XGBoost             | 0.941    | 0.972    | 0.931    | 0.951     |

**Best Model**: Random Forest Classifier with over 95% F1 score and 98% accuracy.

---

## Key Findings
- **Top predictors**: time spent at company, number of projects, monthly hours, last evaluation score, satisfaction level
- **High risk segments**: Employees with long hours, many projects, low satisfaction, and no recent promotion

---

## Data Exploration Insights
- Employees with **low salaries** had significantly higher turnover
- Most who left had **higher workload** (both in hours and project count)
- Satisfaction was **lowest** among employees who left
- **Departments** like Management and HR had the lowest attrition

---

## Recommendations
- **Boost satisfaction**: Conduct regular feedback loops and engagement initiatives
- **Balance workload**: Avoid overburdening high-performing employees
- **Promotions and growth**: Offer advancement or skill-building opportunities
- **Proactive HR**: Use model predictions to identify and support at-risk employees

---

## Next Steps
- Implement SHAP values to enhance interpretability of feature importance
- Deploy the Random Forest model using Flask or Streamlit for real-time HR use
- Incorporate updated or live HR datasets for ongoing evaluation and feedback


---

## Author
Simarpreet Kaur  
[simarpreet-kaur.com](https://simarpreet-kaur.com)
