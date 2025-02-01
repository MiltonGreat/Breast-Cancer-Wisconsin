# Breast Cancer Prediction - Binary Classification

This project aims to build machine learning models to predict whether a tumor is malignant or benign using a dataset of breast cancer cases. The dataset consists of various features extracted from images of fine needle aspirates (FNA) of breast masses.

## Overview

The main goal of this project is to evaluate and compare several classification models on their ability to predict the malignancy of tumors based on the following techniques:

- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Random Forest**

The models are trained and evaluated using cross-validation, hyperparameter tuning, and standard metrics (accuracy, precision, recall, f1-score).

### Dataset Information

The dataset used for training and evaluation is the **Breast Cancer Wisconsin (Diagnostic) dataset**. It contains features such as radius, texture, perimeter, and area of tumors, along with a diagnosis label (malignant or benign). The dataset includes:

- ID number: Unique identifier for each sample
- Diagnosis: Whether the tumor is malignant (M) or benign (B)
- 30 real-valued features: Computed characteristics of cell nuclei, including radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.

## Steps in the Analysis

1. **Data Preprocessing**
    - Data cleaning: Removing irrelevant columns.
    - Encoding the target variable.
    - Handling class imbalance (SMOTE applied).
    - Feature scaling using StandardScaler.

2. **Model Training and Evaluation**
    - Models trained: Logistic Regression, SVM, and Random Forest.
    - Performance metrics: Accuracy, Precision, Recall, F1-Score.
    - Cross-validation and hyperparameter tuning performed on Random Forest.

3. **Results**
    - All models achieved high performance with accuracy above 97%.
    - The Random Forest model showed promising results with hyperparameter tuning, yielding optimal results.

### Results

The models achieve the following accuracy on the test set:

- Logistic Regression: ~97.4%
- SVM: ~964%
- Random Forest Classifier: ~97%

All models perform exceptionally well, with high precision and recall for both classes (malignant and benign).

### Source

Dataset: [Breast Cancer Wisconsin Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
)
