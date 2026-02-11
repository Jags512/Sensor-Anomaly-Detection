# Sensor-Anomaly-Detection

kaggle  link :https://www.kaggle.com/code/jagrutiyuvrajdhangar/sensor-anomaly-detection/edit


📌 Sensor Anomaly Detection using Random Forest
🧠 Project Overview

This project focuses on predicting anomalies based on sensor readings using supervised machine learning techniques. The objective is to build a robust classification model capable of accurately identifying anomalous patterns in tabular sensor data.

The solution emphasizes:

Advanced Exploratory Data Analysis (EDA)

Feature Engineering

Cross-Validation for robustness

Hyperparameter tuning

Performance optimization using F1 Score

🎯 Objective

To classify sensor readings as normal or anomaly (binary/multi-class depending on dataset) using machine learning models.

Evaluation is based on:

Accuracy

Precision

Recall

F1 Score (Primary Metric)

📊 Dataset Description

The dataset consists of:

Multiple sensor feature columns

A target column representing anomaly class

Data Type: Structured tabular data
Problem Type: Classification

🔎 Exploratory Data Analysis

The following preprocessing steps were performed:

✔ Handling missing values using median imputation

✔ Outlier detection using boxplots and IQR

✔ Target distribution analysis

✔ Correlation analysis using heatmap

✔ Feature importance analysis

🛠 Feature Engineering

To enhance model performance, the following features were created:

Sensor mean across all readings

Sensor standard deviation

Interaction-based derived features

Removal of redundant highly correlated features

Feature scaling was applied where necessary.

🤖 Model Used: Random Forest Classifier

Random Forest was selected because:

It handles tabular data effectively

It is robust to outliers

It reduces overfitting via ensemble learning

It provides feature importance for interpretability

🔁 Cross-Validation Strategy

To ensure robustness and avoid overfitting:

Used Stratified K-Fold Cross Validation (k=5)

Maintained class distribution across folds

Evaluated F1 score across all folds

Reported mean F1 score

This ensures the model generalizes well to unseen data.

⚙️ Hyperparameter Tuning

Hyperparameters tuned:

n_estimators

max_depth

min_samples_split

min_samples_leaf

Tuning performed using:

GridSearchCV

Stratified Cross-Validation

F1 score as scoring metric

📈 Model Evaluation

Evaluation Metrics Used:

Accuracy

Precision

Recall

F1 Score (Primary metric)

Confusion Matrix

Final performance was selected based on highest cross-validated F1 score
