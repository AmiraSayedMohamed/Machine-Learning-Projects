# Diabetes Prediction Using Ensemble Learning

## Project Overview

This project aims to predict whether a patient has diabetes based on their medical information, such as glucose levels, BMI, age, and other relevant factors. The prediction is performed using an **ensemble learning** approach, which combines several machine learning models to increase predictive accuracy and robustness. The ensemble consists of the following models:

- **Logistic Regression**
- **Random Forest**
- **XGBoost**
- **Gradient Boosting**
- **Support Vector Machine (SVM)**

The dataset is standardized using **StandardScaler**, and class imbalance in the dataset is addressed with **SMOTE (Synthetic Minority Over-sampling Technique)**.

## Dataset

The dataset used is the **Pima Indians Diabetes Database**, which contains the following columns:

- `Pregnancies`: Number of times pregnant
- `Glucose`: Plasma glucose concentration
- `BloodPressure`: Diastolic blood pressure (mm Hg)
- `SkinThickness`: Triceps skinfold thickness (mm)
- `Insulin`: 2-Hour serum insulin (mu U/ml)
- `BMI`: Body mass index (weight in kg/(height in m)^2)
- `DiabetesPedigreeFunction`: Diabetes pedigree function
- `Age`: Age (years)
- `Outcome`: Target variable (1 for diabetic, 0 for non-diabetic)

The dataset contains 768 rows and 9 columns.

## Project Structure

- **`diabetes_model_sav`**: The saved ensemble model for predicting diabetes.
- **`scaler_sav`**: The saved `StandardScaler` object used for scaling input data.
- **`diabetes.csv`**: The dataset used in this project.

## Steps Followed

1. **Data Preprocessing**:
   - The dataset is split into features (`X`) and target (`y`).
   - SMOTE is applied to address class imbalance by oversampling the minority class.
   - Data is split into training and testing sets.
   - StandardScaler is applied to standardize the feature values.

2. **Ensemble Learning**:
   - A Voting Classifier with soft voting is created, combining Logistic Regression, Random Forest, XGBoost, Gradient Boosting, and SVM.
   - Cross-validation is applied to evaluate model performance on the training data.
   - The final model is trained on the training set and evaluated on the test set.

3. **Model Evaluation**:
   - Model accuracy, confusion matrix, and classification report are generated.
   
4. **Model Saving**:
   - The trained ensemble model and StandardScaler are saved as `diabetes_model_sav` and `scaler_sav` respectively.

## Usage

### 1. Install Dependencies

You need to install the required dependencies to run this project. 
