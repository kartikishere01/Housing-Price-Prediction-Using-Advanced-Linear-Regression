# House Price Prediction using Machine Learning

## Overview

This project presents an end-to-end machine learning solution for predicting residential house prices using the **House Prices: Advanced Regression Techniques** dataset from Kaggle.

The project covers the complete machine learning workflow, including data exploration, preprocessing, model training, model comparison, hyperparameter tuning, and prediction on unseen data.

---

## Problem Statement

The objective of this project is to predict the selling price of residential houses based on various structural and neighborhood-related features.

This is a supervised machine learning problem and is formulated as a regression task.

---

## Dataset

* **Dataset:** House Prices: Advanced Regression Techniques
* **Source:** Kaggle
* **Training Samples:** 1460
* **Test Samples:** 1459
* **Number of Features:** 79
* **Target Variable:** SalePrice

---

## Project Workflow

The project follows a standard machine learning pipeline consisting of the following stages:

1. Problem Definition
2. Data Loading
3. Train-Validation Split
4. Exploratory Data Analysis
5. Data Preprocessing
6. Feature Transformation
7. Pipeline Construction
8. Model Training
9. Model Evaluation
10. Hyperparameter Tuning
11. Final Model Selection
12. Prediction on Test Data

---

## Exploratory Data Analysis

The following analyses were performed:

* Distribution analysis using histograms
* Correlation analysis using Pearson correlation
* Scatter plot analysis for highly correlated features
* Identification of missing values
* Outlier inspection
* Feature relationship analysis

---

## Data Preprocessing

The preprocessing pipeline includes:

* Median imputation for numerical features
* Most frequent imputation for categorical features
* One-Hot Encoding of categorical variables
* Standardization of numerical variables
* Scikit-Learn Pipeline and ColumnTransformer for automated preprocessing

---

## Machine Learning Models

The following regression models were implemented and evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor

---

## Model Performance

| Model                   | Training RMSE | Validation RMSE |
| ----------------------- | ------------: | --------------: |
| Linear Regression       |        19,529 |          29,477 |
| Decision Tree           |             0 |          41,853 |
| Random Forest           |        11,335 |          28,528 |
| Gradient Boosting       |        13,355 |          26,136 |
| Tuned Gradient Boosting |        100.58 |   **24,817.86** |

---

## Hyperparameter Tuning

The best-performing model was optimized using **RandomizedSearchCV** with **5-fold Cross Validation**.

The following hyperparameters were tuned:

* Number of estimators
* Learning rate
* Maximum tree depth
* Minimum samples required for splitting
* Minimum samples per leaf
* Subsampling ratio

---

## Final Results

* **Selected Model:** Gradient Boosting Regressor
* **Validation RMSE:** 24,817.86
* **Kaggle Public Leaderboard Score:** 0.14063

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* SciPy
* Joblib

---

## Repository Structure

```text
House-Price-Prediction/
│
├── data/
│   └── data_description.txt
│
├── models/
│   └── gradient_boosting_model.pkl
│
├── notebooks/
│   └── House_Price_Prediction.ipynb
│
├── submissions/
│   └── submission.csv
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Future Work

Possible improvements to this project include:

* Advanced feature engineering
* Log transformation of the target variable
* Implementation of XGBoost, LightGBM, and CatBoost
* Model ensembling
* Automated feature selection
* Model deployment as a web application

---

## Author

**Kartik Singh**

National Institute of Technology Jalandhar

Machine Learning | Artificial Intelligence | Data Science
