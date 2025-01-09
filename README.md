# Breast Cancer Prediction - Binary Classification

### Overview

This project uses the Breast Cancer Wisconsin (Diagnostic) dataset to practice binary classification techniques and predict whether a tumor is malignant or benign based on various features computed from fine needle aspirate (FNA) images of breast masses.

### Quality Issues

- Imbalanced dataset (malignant cases often fewer than benign).
- Outliers in numerical features due to measurement noise.

Cleaning/Transformation:
- Apply SMOTE (Synthetic Minority Oversampling) for class imbalance.
- Normalize features for SVM or Logistic Regression.

Model Evaluation:
- Focus on recall to minimize false negatives.
- Use AUC-ROC to assess model discrimination.

Dataset Limitations:
- Dataset may not generalize well to different demographics or imaging techniques.

### Dataset Information

The dataset contains features that describe the characteristics of cell nuclei present in breast cancer FNA images. These features were computed from digitized images and used for classification. The dataset includes:

- ID number: Unique identifier for each sample
- Diagnosis: Whether the tumor is malignant (M) or benign (B)
- 30 real-valued features: Computed characteristics of cell nuclei, including radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.

### Project Workflow

 Data Preprocessing:
 - Drop irrelevant columns such as ID.
 - Convert the Diagnosis column to binary values: 1 for malignant (M) and 0 for benign (B).
 - Split the data into features (X) and the target variable (y).

Exploratory Data Analysis (EDA):
- Visualize the class distribution of tumors (malignant vs benign).
- Examine the relationships between the numerical features using heatmaps and pairplots.
- Inspect individual feature distributions.

Model Building and Evaluation:
- Split the dataset into training and testing sets.
- Train and evaluate several classification models, including: Logistic Regression, Support Vector Machine (SVM), Random Forest Classifier
- Evaluate model performance using metrics like accuracy, precision, recall, and F1-score.
- Display the confusion matrix to visualize true positives, false positives, true negatives, and false negatives.

Model Optimization:
- Implement Cross-validation to assess model performance more reliably.
- Perform Hyperparameter tuning using GridSearchCV to optimize the Random Forest model and other classifiers.

### Results

The models achieve the following accuracy on the test set:

- Logistic Regression: ~97.4%
- SVM: ~97.4%
- Random Forest Classifier: ~96.5%

All models perform exceptionally well, with high precision and recall for both classes (malignant and benign).

### Source

https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
