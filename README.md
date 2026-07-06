# Telecom Customer Churn Analysis & Prediction

An end-to-end Data Analytics & Machine Learning project that predicts customer churn and provides actionable business insights through an interactive Power BI dashboard.

## Project Overview

This project analyzes customer behavior using the IBM Telco Customer Churn dataset to identify customers likely to churn. It includes data cleaning, feature engineering, machine learning, and dashboard development to support customer retention strategies.

## Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Power BI (DAX)
- Jupyter Notebook

## Dataset

- **Source:** IBM Telco Customer Churn Dataset (Kaggle)
- **Records:** 7,032 customers
- **Target:** Churn (Yes/No)

## Project Workflow

```
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Machine Learning
      ↓
Model Evaluation
      ↓
Power BI Dashboard
```

## Feature Engineering

- TenureGroup
- AvgRevenuePerMonth
- CustomerValue
- HighRiskCustomer
- ServiceCount

## Machine Learning

Models Compared:
- Logistic Regression (Selected)
- Random Forest

**Evaluation Metrics**
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- 5-Fold Cross Validation

**Best Model**
- Logistic Regression
- Accuracy: **79.32%**
- ROC-AUC: **0.834**

##  Power BI Dashboard

Interactive dashboard featuring:

- KPI Cards
- Churn Analysis by Contract
- Payment Method
- Internet Service
- Tenure Group
- Customer Value
- High-Risk Customer
- Dynamic Filters

##  Key Insights

- Month-to-month customers have the highest churn.
- Fiber optic users churn more than DSL users.
- Electronic check customers show higher churn.
- New customers are significantly more likely to churn.
- Long-term contracts greatly reduce churn.

##  Repository Structure

```
├── data/
├── notebooks/
├── dashboard/
├── presentation/
└── README.md
```

##  Future Improvements

- Deploy the model using Streamlit/FastAPI
- Add SQL-based data pipeline
- Experiment with XGBoost & SHAP

---

**Author:** Tushar Vaidya 

24je0471
B.Tech Mining Engineering, IIT (ISM) Dhanbad
