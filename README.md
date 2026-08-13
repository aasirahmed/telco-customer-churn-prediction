# Telco Customer Churn Prediction

## 📌 Overview

This project builds a machine learning classification model to predict whether a telecommunications customer is likely to churn.

The project uses Logistic Regression to analyze customer demographics, account information, services, contract details, and billing information to predict customer churn.

## 🎯 Objective

The objective is to identify customers who are likely to leave the service, helping businesses understand churn patterns and potentially take proactive customer-retention actions.

## 🗂️ Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information such as:

- Customer demographics
- Tenure
- Contract type
- Internet services
- Payment method
- Monthly charges
- Total charges
- Churn status

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Joblib
- Google Colab

## 🔄 Machine Learning Workflow

``text
Raw Dataset
     ↓
Data Exploration
     ↓
Data Cleaning
     ↓
Feature / Target Separation
     ↓
Categorical Encoding
     ↓
Train-Test Split
     ↓
Feature Scaling
     ↓
Logistic Regression
     ↓
Prediction
     ↓
Probability Estimation
     ↓
Model Evaluation

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Converted `TotalCharges` into numeric format.
2. Handled missing values.
3. Removed `customerID` because it is an identifier and not a predictive feature.
4. Separated `Churn` as the target variable.
5. Converted `Churn` from `Yes/No` into `1/0`.
6. Applied one-hot encoding to categorical variables.
7. Split the data into training and testing sets.
8. Applied `StandardScaler` to the feature data.

## 🤖 Model

The project uses **Logistic Regression** for binary classification.

The model predicts the probability of customer churn and uses that probability to classify customers as either:

- `0` → No Churn
- `1` → Churn

## 📊 Results

The Logistic Regression model achieved approximately **82% accuracy** on the test dataset.

| Class | Precision | Recall | F1-Score |
|------|-----------|--------|----------|
| No Churn | 0.86 | 0.90 | 0.88 |
| Churn | 0.69 | 0.60 | 0.64 |

The results show that the model performs better at identifying customers who do not churn than customers who do churn.

## 🔮 Example Prediction

The model can also estimate the probability of churn for an individual customer.

Example:

```text
Churn Probability: ~69%
Prediction: Churn

