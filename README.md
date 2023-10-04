# Classification-by-Consent-Flag-using-Random-Forest-and-XGBoost WITH and WITHOUT Data Augumentation Techniques

## Introduction
This repository contains code and data for predicting customer behavior in an online store. The primary objective of this project is to predict whether a given customer will make a purchase (1) or not (0) in the store. We explore two different classification models: Random Forest and XGBoost.
 
## Objectives
Exploratory Data Analysis (EDA): We investigate the data to gain insights into its characteristics and distributions.

1. Imported Necessary Libraries: We've imported libraries like pandas, numpy, sklearn, imbalanced-learn (for data augmentation), RandomForestClassifier, xgboost, and others.

2. Exploratory Data Analysis (EDA): We've loaded the dataset, displayed its head, described statistical information, and checked for missing values.
   
3. Data Preparation: This step focuses on data preprocessing, ensuring that it is clean and suitable for modeling. Tasks include handling missing values, one-hot encoding categorical features, and label encoding binary features.

4. Balancing the Dataset: We've applied different data augmentation techniques like Random Oversampling, Borderline SMOTE, ADASYN, and SMOTE to address class imbalance.

5. Model Training: We train two classification models, Random Forest, and XGBoost. Random Forest and XGBoost models were trained whithout using and using the augmented datasets.

6. Cross-Validation: Cross-validation was performed for the XGBoost model using ADASYN, Borderline Smote, SMOTE, and Random Oversampling and its performance was assessed.

7. Model Evaluation: To assess model performance, we use evaluation metrics such as precision, recall, and F1-score. We also address class imbalance issues to ensure fair evaluation.

5. Model Selection: After evaluating both Random Forest and XGBoost models, we make an informed decision to select the most appropriate model for predicting customer purchases in the online store.

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

## Model Performance

### XGBoost Model
The XGBoost Classifier(using cross-validation) with Random Oversampling demonstrated the best overall performance with an accuracy of 95%, precision for Class 0 (99%), Precision for Class 1 (0.92%), 
Recall for Class 0(91%), Recall for Class 1 (99%), F1-score for Class 0 (95%), F1-score for Class 1 (96%). 
The use of stratify parameter during the random oversampling ensured that the class distribution in the target variable was maintained, preventing bias in the oversampled dataset and contributing to the model's excellent performance.

## Conclusion 
In conclusion, this project successfully addressed the challenge of predicting customer behavior. By exploring Random Forest and XGBoost models, applying data augmentation techniques, and conducting cross validation, we have developed effective predictive models. These models can assist in targeting potential customers more effectively and improving conversion rates. 

## Credits
This project was implemented by Aleksandar Dimitrov and is licensed under the MIT License. If you have any questions or comments, please feel free to contact me at alexi.zein@gmail.com.
