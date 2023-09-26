# Classification-by-Consent-Flag-using-Random-Forest-and-XGBoost

## Introduction
This repository contains code and data for predicting customer behavior in an online store. The primary objective of this project is to predict whether a given customer will make a purchase (1) or not (0) in the store. We explore two different classification models: Random Forest and XGBoost.
 
## Objectives
Exploratory Data Analysis (EDA): We investigate the data to gain insights into its characteristics and distributions.

1. Data Preparation: This step focuses on data preprocessing, ensuring that it is clean and suitable for modeling. Tasks include handling missing values, one-hot encoding categorical features, and label encoding binary features.

2. Model Training: We train two classification models, Random Forest, and XGBoost.

3. Model Evaluation: To assess model performance, we use evaluation metrics such as precision, recall, and F1-score. We also address class imbalance issues to ensure fair evaluation.

4. Model Selection: After evaluating both Random Forest and XGBoost models, we make an informed decision to select the most appropriate model for predicting customer purchases in the online store.

## Getting Started
Prerequisites
To run the code in this repository, you'll need the following Python libraries:

pandas
numpy
sklearn
xgboost
matplotlib
seaborn

## Data
The dataset used in this project is stored in a CSV file named 1.csv. You can replace this with your own dataset or modify the code to load a different dataset.

## Data Preprocessing
The data preparation process involves steps like separating inputs and target variables, one-hot encoding categorical features, and label encoding binary features. The code in this repository provides detailed examples of how to perform these tasks.

## Model Training and Evaluation
Two classification models, Random Forest and XGBoost, are trained and evaluated in this project. The code includes training the models, making predictions, and generating classification reports and confusion matrices.

## Results

1. Random Forest Model
The Random Forest model achieved the following results on the test data:

Accuracy: 89%
Precision: 91% for Class 0, 75% for Class 1
Recall: 96% for Class 0, 53% for Class 1
F1-score: 94% for Class 0, 62% for Class 1

2. XGBoost Model
The XGBoost model achieved the following results on the test data:

Accuracy: 90%
Precision: 93% for Class 0, 71% for Class 1
Recall: 96% for Class 0, 58% for Class 1
F1-score: 94% for Class 0, 64% for Class 1

## Conclusion
This project demonstrates how to predict customer behavior in an online store using machine learning techniques. Both Random Forest and XGBoost models show promising results in identifying potential customers who are likely to make purchases. You can use this code as a starting point for your own customer behavior prediction tasks.

## Credits
This project was implemented by Aleksandar Dimitrov and is licensed under the MIT License. If you have any questions or comments, please feel free to contact me at alexi.zein@gmail.com.
