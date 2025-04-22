# 🧠 Employee Attrition Analysis using Logistic Regression

This repository contains a comprehensive data science project focused on analyzing and predicting employee attrition using a logistic regression model. The aim is to identify key drivers of attrition and help businesses develop proactive employee retention strategies.

---

## 📊 Project Overview

**Objective:**  
To build a predictive model to classify whether an employee is likely to stay or leave, and to uncover actionable insights through detailed exploratory and statistical analysis.

**Dataset:**  
- 74,610 employee records
- Features include demographics, job roles, compensation, satisfaction levels, and company characteristics
- Target variable: `Attrition` (Stayed / Left)

---

## 🛠️ Workflow Summary

### 1. Data Preprocessing
- Missing values handled in `Distance from Home` (2.56%) and `Company Tenure (3.23%)`
- One-hot encoding applied to categorical variables
- Numerical features standardized (mean = 0, std = 1)

### 2. Exploratory Data Analysis (EDA)
- Attrition is higher among females, singles, and entry-level employees
- Poor Work-Life Balance, Low Job Satisfaction, and Overtime strongly correlate with churn
- Remote work and positive company reputation improve retention

### 3. Feature Engineering
- Recursive Feature Elimination (RFE) selected top 15 features
- VIF analysis confirmed no multicollinearity among features

### 4. Model Training & Evaluation
- Model: **Logistic Regression**
- AUC (ROC Curve): **0.83**
- Average Precision Score (PR Curve): **0.817**
- Balanced performance with optimal threshold at **~0.5**
- Key predictors include:
  - 🔺 `Overtime`, `Poor Work-Life Balance`, `Single Marital Status` → Higher Attrition
  - 🔻 `Remote Work`, `PhD Education`, `Senior Job Level` → Lower Attrition

---

## ✅ Key Insights

- Remote and flexible work arrangements significantly reduce attrition
- Work-life balance and employee recognition are actionable retention levers
- Seniority and educational level contribute to employee stability
- The model is interpretable, robust, and suitable for production deployment

---

## 📁 Files in this Repo

| File | Description |
|------|-------------|
| `Predicting_Employee_Retention_Starter.ipynb` | Full code for data prep, EDA, modeling, and evaluation |
| `Final_Employee_Attrition_Analysis_Report_SoumyajitBera.pdf` | Detailed multi-page report |
| `data/Employee_data.csv` | Input dataset  |
| `README.md` | Project documentation |



