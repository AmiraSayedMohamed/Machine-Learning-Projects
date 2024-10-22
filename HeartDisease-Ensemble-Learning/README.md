# Heart Disease Prediction Project

## Overview
This project aims to predict the presence of heart disease in patients based on various medical attributes. The model is built using an ensemble learning approach to improve prediction accuracy.

## Steps

1. **Exploratory Data Analysis (EDA)**:
   - Conducted an initial analysis of the dataset to understand its structure, distribution of features, and relationships between variables.
   - Visualizations were created to identify trends and patterns in the data.

2. **Data Preparation**:
   - The dataset was cleaned and processed to handle any missing values and outliers.
   - Features were separated into input variables (X) and the target variable (y).

3. **Train-Test Split**:
   - The dataset was split into training and testing sets, with 80% of the data used for training and 20% for testing.

4. **Model Initialization**:
   - The following classifiers were initialized:
     - **Logistic Regression**: A linear model for binary classification.
     - **Support Vector Machines (SVM)**: A model that finds the hyperplane to separate classes.
     - **K-Nearest Neighbors (KNN)**: A non-parametric method used for classification based on the closest training examples.
     - **XGBoost**: An optimized gradient boosting library designed for performance and speed.
     - **Gradient Boosting Classifier**: An ensemble technique that builds models sequentially to reduce errors.

5. **Ensemble Learning with Voting Classifier**:
   - A Voting Classifier was created using the above models, applying soft voting to aggregate predictions based on predicted probabilities.

6. **Model Training**:
   - The Voting Classifier was trained using the training dataset.

7. **Cross-Validation**:
   - Cross-validation was performed to evaluate the model's performance and ensure its robustness.

8. **Model Evaluation**:
   - Predictions were made on the test set, and a classification report was generated to assess the model's accuracy, precision, recall, and F1 score.

## Conclusion
The heart disease prediction model leverages multiple algorithms to enhance predictive accuracy and reliability. Further improvements can be made by fine-tuning hyperparameters and exploring additional data preprocessing techniques.

