**Telecom Customer Churn & Retention Analysis**

# Project Overview

Customer churn is a major challenge for telecom companies because losing existing customers can negatively impact recurring revenue and increase customer acquisition requirements.
This project analyzes telecom customer data to identify **customer churn patterns, high-risk segments, and factors associated with customer attrition**.
The project combines **Python-based statistical analysis and Logistic Regression** with an interactive **Power BI dashboard** to translate customer data into actionable business insights.

##  Dataset

**Dataset:** IBM Telco Customer Churn Dataset

The project uses a publicly available telecom customer churn dataset containing customer demographics, service subscriptions, contract information, billing details and churn status.

---

# Business Objectives

The analysis aims to answer:

- What is the overall customer churn rate?
- Which contract types have the highest churn?
- How does customer tenure relate to churn?
- Which internet service categories show higher churn?
- Which payment methods are associated with higher churn?
- How does monthly charging relate to churn?
- Which customer segments should be prioritized for retention?

---

# Tools & Technologies

## Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Power BI
- Data transformation
- DAX measures
- KPI development
- Interactive dashboards
- Data visualization
- Customer segmentation

## Other
- GitHub for project documentation and version control

---

#  Analytical Approach

## 1. Data Preparation

The telecom customer dataset was imported and prepared for analysis.

Key preprocessing steps included:

- Preparing categorical variables for modelling
- Creating dummy variables for categorical features
- Defining independent and dependent variables
- Splitting the dataset into training and testing sets

---

## 2. Exploratory Data Analysis

Customer churn was analyzed across multiple dimensions, including:

- Contract type
- Customer tenure
- Internet service
- Payment method
- Monthly charges
- Customer characteristics
- Additional subscribed services

The analysis was used to identify customer segments with relatively higher and lower churn rates.

---

## 3. Predictive Modelling

A **Logistic Regression model** was developed to estimate the likelihood of customer churn.

The model was evaluated using:

- Accuracy
- Precision
- Recall
- Confusion Matrix
- ROC-AUC

## Model Performance

| Metric | Result |
|---|---:|
| Accuracy | **79.45%** |
| Precision | **62.24%** |
| Recall | **55.60%** |
| ROC-AUC | **84.43%** |

<img width="547" height="413" alt="image" src="https://github.com/user-attachments/assets/bdf2eac6-024f-4094-9cbb-da406ace8e70" />

The model achieved an ROC-AUC of **84.43%**, indicating good ability to distinguish between customers who churn and those who do not.

However, the recall of **55.60%** indicates that there is scope to improve the identification of actual churners, particularly when minimizing missed churn-risk customers is a business priority.

## Confusion Matrix

| | Predicted: No Churn | Predicted: Churn |
|---|---:|---:|
| **Actual: No Churn** | 1,827 | 250 |
| **Actual: Churn** | 329 | 412 |

<img width="627" height="534" alt="image" src="https://github.com/user-attachments/assets/f5fe3e63-756b-4c8e-9cff-1823e65d9814" />

The model correctly identified **412 churned customers**, while **329 actual churners were not identified** by the model.

---

## 4. Feature Analysis

The Logistic Regression coefficients were examined to understand the direction of association between customer attributes and churn.

Some of the notable positive coefficients were:

| Variable | Coefficient |
|---|---:|
| Month-to-month | **0.984** |
| Fiber optic | **0.547** |
| One year | **0.520** |
| Paperless Billing | **0.239** |
| Multiple Lines | **0.216** |
| Electronic check | **0.299** |

Notable negative coefficients included:

| Variable | Coefficient |
|---|---:|
| Phone Service | **-1.314** |
| Online Security | **-0.546** |
| Tech Support | **-0.439** |
| Online Backup | **-0.293** |
| Device Protection | **-0.263** |
| Tenure | **-0.037** |

These coefficients indicate associations within the fitted model and should not be interpreted as causal effects.

---

## Power BI Dashboard

An interactive Power BI dashboard was developed to provide a business-focused view of customer churn.

# Dashboard KPIs

- Total Customers
- Churned Customers
- Overall Churn Rate
- Average Monthly Charges
- Average Customer Tenure

# Dashboard Analysis

The dashboard analyzes churn by:

- Contract Type
- Internet Service
- Customer Tenure
- Monthly Charges
- Payment Method

Interactive slicers allow users to filter the analysis by key customer attributes.

---

## Key Business Insights

# 1. Contract Type

Month-to-month customers show a **42.71% churn rate**, compared with **11.27% for one-year contracts** and **2.83% for two-year contracts**.

This indicates that customers without long-term commitments represent an important retention segment.

# 2. Customer Tenure

Customers with **0–12 months of tenure have the highest churn rate at 47.44%**.

Churn decreases as tenure increases, reaching **9.51% among customers with 49+ months of tenure**.

This highlights the first year of the customer lifecycle as an important retention window.

# 3. Internet Service

Fiber optic customers show a **41.89% churn rate**, compared with **18.96% for DSL** and **7.40% for customers without internet service**.

The higher churn observed among fiber optic customers warrants further investigation into pricing, service quality, customer experience and competitive alternatives.

# 4. Payment Method

Customers using **electronic check have the highest churn rate at 45.29%** among the payment methods analyzed.

This segment could be investigated further to understand whether payment experience or customer characteristics contribute to the higher observed churn.

---

## Business Recommendations

# 1. Strengthen Early-Tenure Retention

Develop stronger onboarding, engagement and customer-support initiatives during the first 12 months, when churn is highest.

# 2. Encourage Longer-Term Contracts

Develop targeted retention offers and incentives to encourage month-to-month customers to move toward one-year or two-year contracts.

# 3. Investigate High-Churn Service Segments

Further investigate the customer experience, pricing, service quality and competitive environment associated with fiber optic customers.

# 4. Review Payment Experience

Investigate whether electronic-check customers experience payment friction or represent a particular high-risk customer segment.

# 5. Improve Churn-Risk Identification

The model's **84.43% ROC-AUC** demonstrates useful discriminatory ability, but the **55.60% recall** indicates that additional modelling, feature engineering or threshold optimization could improve identification of customers at risk of churn.

---
# Skills Demonstrated

Data Analysis | Data Cleaning | Exploratory Data Analysis | Statistical Modelling | Logistic Regression | Model Evaluation | Python | Pandas | NumPy | Scikit-learn | Power BI | DAX | Data Visualization | Customer Segmentation | Business Insights



