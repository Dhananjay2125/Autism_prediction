
## Autism prediction system
## Introduction

The Autism Prediction System is a machine learning project designed to predict autism risk using various personal and behavioral factors. Built in Google Colaboratory, this project involves data preprocessing, exploratory data analysis (EDA), handling class imbalance, and model training with hyperparameter tuning. The system is optimized to provide accurate predictions and includes label encoding and SMOTE for better handling of imbalanced data.
## Features
- Automated handling of missing values in critical columns (ethnicity, relation).
- Detection and removal of irrelevant columns (e.g., age_desc).
- Identification and resolution of class imbalance in target and categorical features.
- Exploratory Data Analysis (EDA) with insights into numerical and categorical data.
- Outlier detection using boxplots.
- Efficient preprocessing with label encoding, encoder storage, and SMOTE application.
- Model selection, hyperparameter tuning, and evaluation on test data.

## Technologies Used
- Environment: Google Colaboratory
- Programming Language: Python
- Libraries:
    - pandas
    - numpy
    - matplotlib
    - seaborn
    - scikit-learn
    - imbalanced-learn
    - pickle

## Workflow
1. Data Inspection & Cleaning
    - Import essential libraries.
    - Load the dataset and inspect its structure.
    - Handle missing values in ethnicity and relation columns.
    - Remove irrelevant column (age_desc) and fix inconsistencies in the country column.
    - Address class imbalance in the target column.
2. Exploratory Data Analysis (EDA)
- Univariate Analysis:
    - Numerical columns: Analyze distributions and detect outliers using boxplots.
    - Categorical columns: Analyze frequency distributions.
- Bivariate Analysis:
    - Investigate relationships between features and the target variable.
- Insights:
- Identified outliers in age and result columns.
- Addressed class imbalance in categorical features and target.
- No highly correlated columns were found.
3. Data Preprocessing
- Apply label encoding to categorical columns and store the encoders as pickle files.
- Handle imbalanced data using SMOTE.
4. Model Training and Evaluation
- Split the data into training and testing sets.
- Train multiple models with hyperparameter tuning to select the best-performing model.
- Save the trained model for future use.
- Evaluate the model on test data using metrics such as accuracy, precision, recall, and F1-score.