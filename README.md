**Autism Predictor**

Autism Predictor is a machine learning project that predicts Autism Spectrum Disorder (ASD) using screening questionnaire responses and demographic features. The project focuses on proper data preprocessing, class imbalance handling, model comparison, and hyperparameter tuning to build a reliable predictive model.

**Project Overview**

The goal of this project is to:

Analyze screening questionnaire data

Handle outliers using IQR-based replacement

Encode categorical features

Balance class distribution using SMOTE

Train and compare multiple classification models

Select and save the best performing model

This repository contains the full training pipeline along with the trained model and encoders for reproducibility.

**Dataset**

The dataset includes:

A1_Score to A10_Score (screening questionnaire responses)

Age

Gender

Ethnicity

Jaundice

Autism history

Country of residence

App usage history

Relationship

Target variable (Class/ASD)

The dataset used for training is included in this repository.

**Preprocessing Steps**

The following preprocessing steps were performed:

Handling missing values (if any)

Outlier detection and replacement using the IQR method

Label encoding of categorical variables

Train-test split

Class balancing using SMOTE

**Models Used**

The following models were trained and evaluated:

Decision Tree

Random Forest

XGBoost

Cross-validation was used to evaluate model performance. Hyperparameter tuning was performed using RandomizedSearchCV.

The best performing model was selected and saved as:

best_model.pkl

Encoders used during preprocessing are saved as:

encoders.pkl

**Results**

The models were evaluated using cross-validation accuracy. Random Forest and XGBoost showed strong performance after hyperparameter tuning. The final model was selected based on the highest validation accuracy.

**Future Improvements**

Add a web interface using Flask or Streamlit

Deploy the model to a cloud platform

Perform additional feature engineering

Try ensemble stacking methods
