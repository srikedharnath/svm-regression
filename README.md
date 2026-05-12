# svm-regression

# Insurance Charges Prediction using Support Vector Regression (SVR)

## Overview

This project predicts medical insurance charges using Support Vector Regression (SVR).  
The prediction is based on personal and health-related features such as age, gender, BMI, smoking status, region, and number of children.

This project demonstrates:
- Data preprocessing
- Label Encoding
- Feature Scaling
- Train-Test Split
- SVR Model Training
- Model Evaluation

---

# Dataset Information

The dataset contains 1338 rows and 7 columns.

## Features

| Column Name | Description |
|-------------|-------------|
| age | Age of the person |
| sex | Gender |
| bmi | Body Mass Index |
| children | Number of children |
| smoker | Smoking status |
| region | Residential region |
| charges | Medical insurance charges |

---

# Problem Type

This is a Regression problem because the target variable (`charges`) contains continuous numerical values.

---

# Machine Learning Algorithm Used

- Support Vector Regression (SVR)

---

# Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

# Project Workflow

1. Load Dataset
2. Understand Dataset
3. Check Null Values
4. Encode Categorical Data
5. Feature Scaling
6. Split Features and Target
7. Train-Test Split
8. Train SVR Model
9. Predict Output
10. Evaluate Model

---

# Data Preprocessing

## Label Encoding

The following categorical columns were encoded:
- sex
- smoker
- region

---

# Feature Scaling

StandardScaler was used because SVR is sensitive to feature ranges.

---

# SVR Hyperparameters Used

```python
SVR(
    kernel='rbf',
    C=100,
    gamma=0.1,
    epsilon=0.1
)
