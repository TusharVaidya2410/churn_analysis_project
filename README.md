
# Telecom Customer Churn Analysis & Prediction

> **An end-to-end Data Analytics & Machine Learning project that predicts customer churn, uncovers the key drivers behind customer attrition, and translates insights into an interactive Power BI dashboard for business decision-making.**

---

## Project Overview

Customer churn is one of the biggest challenges faced by telecom companies, as acquiring a new customer is significantly more expensive than retaining an existing one.

This project analyzes customer behavior using the IBM Telco Customer Churn dataset, engineers business-driven features, compares multiple machine learning models, and presents actionable insights through an interactive Power BI dashboard.

The goal is not only to predict which customers are likely to churn but also to understand **why they churn** and provide data-driven recommendations for improving customer retention.

---

## Objectives

* Analyze customer behavior and identify churn patterns.
* Perform data cleaning and feature engineering.
* Build and compare Machine Learning models.
* Evaluate models using multiple performance metrics.
* Develop an interactive Power BI dashboard for business users.
* Generate actionable business recommendations for customer retention.

---

## Dataset

* **Source:** IBM Telco Customer Churn Dataset (Kaggle)
* **Records:** 7,032 Customers
* **Target Variable:** Churn (Yes / No)
* **Class Distribution:**

  * No Churn: **73.42%**
  * Churn: **26.58%**

---

# Tech Stack

### Programming

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

### Data Visualization

* Power BI
* DAX Measures

### Development Environment

* Jupyter Notebook
* VS Code

### Version Control

* Git
* GitHub

---

#  Project Workflow

```text
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Engineering
      │
      ▼
Encoding & Preprocessing
      │
      ▼
Train-Test Split
      │
      ▼
Machine Learning Models
      │
      ▼
Model Evaluation
      │
      ▼
Power BI Dashboard
      │
      ▼
Business Insights
```

---

#  Exploratory Data Analysis

The project investigates customer churn across multiple business dimensions including:

* Contract Type
* Internet Service
* Payment Method
* Monthly Charges
* Tenure
* Customer Value
* Customer Demographics

The analysis revealed several clear churn patterns that informed both feature engineering and business recommendations.

---

#  Feature Engineering

To improve model performance and business interpretability, several custom features were created.

### • TenureGroup

Groups customers into lifecycle stages:

* New
* Growing
* Established
* Loyal

---

### • AvgRevenuePerMonth

Normalizes customer spending by tenure.

```text
Total Charges
──────────────
    Tenure
```

---

### • ServiceCount

Counts the number of subscribed telecom services.

---

### • CustomerValue

Segments customers into value tiers for business analysis.

---

### • HighRiskCustomer

Flags customers combining multiple churn risk factors:

* Month-to-month contract
* Electronic check payment
* No Online Security

---

# Machine Learning Models

Two supervised learning algorithms were trained and compared.

## Logistic Regression

* Accuracy: **79.32%**
* ROC-AUC: **0.834**
* Better recall on churn class
* Selected as the final model

---

## Random Forest

* Accuracy: **78.39%**
* Feature Importance Analysis
* Used for comparison and model interpretation

---

# Model Evaluation

Evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix
* 5-Fold Stratified Cross Validation

Since the dataset is moderately imbalanced (73:27), model selection was based not only on accuracy but also on **ROC-AUC and Recall**, as identifying potential churn customers is more valuable than maximizing overall accuracy.

---

# Feature Importance

The Random Forest model identified the most influential features for predicting churn:

* Total Charges
* Average Revenue Per Month
* Tenure
* Monthly Charges
* High Risk Customer
* Internet Service
* Service Count

---

# Power BI Dashboard

An interactive dashboard was developed to help business users explore churn behavior.

### Dashboard Features

* KPI Cards
* Churn Rate
* Contract Analysis
* Internet Service Analysis
* Payment Method Analysis
* Tenure Group Analysis
* Customer Value Distribution
* High Risk Customer Analysis
* Interactive Filters
* Business Insight Panel

---

# Key Business Insights

* Month-to-month customers exhibit the highest churn rate.
* Fiber optic customers churn significantly more than DSL users.
* Electronic check users show substantially higher churn than other payment methods.
* Customers in their first year are the most likely to leave.
* High-risk customers require immediate retention efforts.
* Long-term contracts significantly reduce customer churn.

---

# Business Recommendations

* Encourage customers to switch to long-term contracts.
* Improve onboarding during the first year of service.
* Investigate issues affecting fiber optic customers.
* Improve the electronic payment experience.
* Focus retention campaigns on high-risk customer segments.

---

# Future Improvements

* Deploy the model using Streamlit or FastAPI.
* Integrate SQL for automated data extraction from production databases.
* Experiment with XGBoost and LightGBM.
* Apply SHAP for explainable AI.
* Implement real-time churn prediction.

---

# Repository Structure

```text
 Telecom-Customer-Churn-Analysis
│
├── data/
│   ├── Customer_Churn.csv
│   └── Customer_Churn_Cleaned.csv
│
├── notebooks/
│   └── 01-data_understanding.ipynb
│
├── dashboard/
│   └── Telecom_Churn_Dashboard.pbix
│
├── presentation/
│   └── Project_Presentation.pdf
│
├── images/
│   ├── dashboard.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
└── README.md
```

---

#  Author

**Tushar Ravindra Vaidya**
24je0471

B.Tech Mining Engineering

Indian Institute of Technology (ISM), Dhanbad
