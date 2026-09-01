# Customer Churn Prediction

## 📌 Project Overview

This project predicts whether a customer is likely to churn using machine learning classification techniques.

The project includes data cleaning, exploratory data analysis, feature preprocessing, model training, model evaluation, model comparison, and final churn prediction.

## 🎯 Objective

The main objective is to identify customers who are likely to churn based on customer demographics, usage behavior, support interactions, payment delays, subscription details, spending, and interaction history.

## 📊 Dataset

The dataset contains customer-level information including:

- Customer ID
- Age
- Gender
- Tenure
- Usage Frequency
- Support Calls
- Payment Delay
- Subscription Type
- Contract Length
- Total Spend
- Last Interaction
- Churn

The model-training dataset contains **64,374 records**.

The final prediction dataset contains **203,375 customer records** after cleaning.

## 🔍 Exploratory Data Analysis

The project analyzed:

- Churn distribution
- Support calls by churn status
- Payment delay by churn status
- Total spend by churn status
- Age by churn status
- Tenure by churn status
- Usage frequency by churn status
- Last interaction by churn status
- Churn percentage by gender
- Feature correlations with churn

### Important findings

Customers who churned had, on average:

- Higher support calls
- Higher payment delays
- Higher average age
- Higher tenure
- Lower usage frequency
- Lower total spend

Payment Delay showed the strongest correlation with churn among the numerical variables analyzed.

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Checked missing values
2. Removed completely empty rows
3. Checked duplicate Customer IDs
4. Checked duplicate rows
5. Separated features and target
6. Identified categorical and numerical features
7. Handled missing numerical values using training-data medians
8. Encoded categorical variables
9. Prepared data for machine learning

Categorical features:

- Gender
- Subscription Type
- Contract Length

Numerical features:

- Age
- Tenure
- Usage Frequency
- Support Calls
- Payment Delay
- Total Spend
- Last Interaction

After encoding, the feature matrix contained **15 features**.

## 🤖 Machine Learning Models

Two classification models were evaluated:

### 1. Logistic Regression

### 2. Random Forest

## 📈 Model Evaluation

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 63.35% | 98.23% | 36.02% | 52.71% | 83.53% |
| Random Forest | 58.37% | 98.11% | 27.12% | 42.49% | 80.49% |

## 🏆 Final Model

**Logistic Regression** was selected as the final model based on the highest F1 Score and ROC-AUC among the evaluated models.

### Final performance

- Accuracy: **63.35%**
- Precision: **98.23%**
- Recall: **36.02%**
- F1 Score: **52.71%**
- ROC-AUC: **83.53%**

## 📁 Project Files

```text
customer-churn-prediction/
│
├── README.md
├── customer_churn_dataset-training-master.csv
├── customer_churn_dataset-testing-master.csv
├── final_customer_churn_predictions.csv
├── model_evaluation_metrics.csv
└── feature_importance.csv
