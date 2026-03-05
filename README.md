# Diabetes Prediction using Support Vector Machine (SVM)

This notebook demonstrates how to build a Support Vector Machine (SVM) model to predict diabetes based on various health parameters. The model is trained and evaluated using the `diabetes.csv` dataset.

## Project Overview

The goal of this project is to classify individuals as diabetic or non-diabetic using an SVM classifier. Key steps include data preprocessing, model training, and evaluation.

## Dataset

The dataset used is `diabetes.csv`, which contains several medical predictor variables and one target variable, `Outcome`, indicating whether the patient has diabetes (1) or not (0).

## Libraries Used

*   **pandas**: For data manipulation and analysis.
*   **numpy**: For numerical operations.
*   **scikit-learn**: For machine learning tasks, including data splitting, standardization, SVM model, and accuracy metrics.

## Steps Involved

1.  **Data Loading and Initial Exploration**: The `diabetes.csv` file is loaded into a pandas DataFrame. Basic data exploration such as `head()`, `shape`, `describe()`, and `value_counts()` for the `Outcome` column are performed.
2.  **Data Preprocessing**: 
    *   Features (X) and target (Y) are separated.
    *   Data standardization is applied using `StandardScaler` to bring all features to a similar scale.
3.  **Data Splitting**: The dataset is split into training and testing sets (80% training, 20% testing) using `train_test_split`, ensuring a stratified split based on the `Outcome` variable.
4.  **SVM Model Training**: A Support Vector Machine classifier with a linear kernel is initialized and trained on the standardized training data.
5.  **Model Evaluation**: The trained model's accuracy is evaluated on both the training and test datasets.
6.  **Prediction on New Data**: The model demonstrates how to make predictions on new, unseen data after standardizing it.
