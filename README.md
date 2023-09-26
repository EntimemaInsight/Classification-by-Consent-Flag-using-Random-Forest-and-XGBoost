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

## Model Performance

**Random Forest Model**

Confusion Matrix (Random Forest): The confusion matrix for the Random Forest model provides further insights into its performance. It shows:
True Positives (TP): 53% of actual purchases were correctly predicted as purchases.
True Negatives (TN): 96% of actual non-purchases were correctly predicted as non-purchases.
False Positives (FP): 9% of non-purchases were incorrectly predicted as purchases.
False Negatives (FN): 47% of actual purchases were incorrectly predicted as non-purchases.

The Random Forest model achieved an accuracy of 89%, which indicates that it correctly classified 89% of the instances in the test dataset. The precision for Class 0 is impressive at 91%, meaning that when the model predicts a customer won't make a purchase (Class 0), it is accurate 91% of the time. However, the precision for Class 1 is lower at 75%, suggesting that when the model predicts a purchase (Class 1), it is accurate only 75% of the time. This discrepancy highlights the model's tendency to overpredict non-purchases.

The recall for Class 0 is excellent at 96%, indicating that the model identifies 96% of actual non-purchases. In contrast, the recall for Class 1 is lower at 53%, revealing a notable weakness in detecting actual purchases. This imbalance in precision and recall between the two classes reflects the challenge of imbalanced data, where the model is inclined to classify most instances as non-purchases due to the predominance of Class 0 in the dataset.

Confusion Matrix (Random Forest):

The confusion matrix for the Random Forest model provides further insights into its performance. It shows:

True Positives (TP): 53% of actual purchases were correctly predicted as purchases.
True Negatives (TN): 96% of actual non-purchases were correctly predicted as non-purchases.
False Positives (FP): 9% of non-purchases were incorrectly predicted as purchases.
False Negatives (FN): 47% of actual purchases were incorrectly predicted as non-purchases.
XGBoost Model
The XGBoost model demonstrated slightly better overall performance with an accuracy of 90%. Similar to the Random Forest model, it excels in precision for Class 0 (93%) but struggles with precision for Class 1 (71%). The recall for Class 0 remains high at 96%, while the recall for Class 1 is still relatively low at 58%.

Confusion Matrix (XGBoost):

The confusion matrix for the XGBoost model provides additional insights into its performance. It shows:

True Positives (TP): 58% of actual purchases were correctly predicted as purchases.
True Negatives (TN): 96% of actual non-purchases were correctly predicted as non-purchases.
False Positives (FP): 7% of non-purchases were incorrectly predicted as purchases.
False Negatives (FN): 42% of actual purchases were incorrectly predicted as non-purchases.
Cross-Validation for XGBoost
An important improvement in the XGBoost model's evaluation is the use of cross-validation. This technique involves splitting the training data into multiple subsets and performing training and validation iteratively. It provides a more robust assessment of model performance by reducing the risk of overfitting to the training data.

Cross-Validation Results (XGBoost):

With cross-validation applied to the XGBoost model, we observe a consistent performance across multiple folds. The accuracy remains at 90%, and precision, recall, and F1-score are consistent with the non-cross-validated results. This indicates that the model's performance is stable and not heavily influenced by the specific training-validation split, enhancing our confidence in its effectiveness.

In conclusion, while both Random Forest and XGBoost models show promise in predicting customer behavior, addressing the imbalance in the dataset and fine-tuning model parameters are essential steps for enhancing the accuracy of predictions, particularly for Class 1 (customer purchases). The inclusion of confusion matrices provides a more granular view of the models' performance, and the use of cross-validation for XGBoost strengthens the reliability of our evaluation. Additional domain-specific insights and features could further contribute to better model performance in real-world scenarios.





## Conclusion
In this customer behavior prediction project, we evaluated two machine learning models: Random Forest and XGBoost. These models were employed to predict whether a customer would make a purchase (Class 1) or not (Class 0) in an online store. The results provide valuable insights into the effectiveness of the models and the challenges posed by imbalanced data.

## Credits
This project was implemented by Aleksandar Dimitrov and is licensed under the MIT License. If you have any questions or comments, please feel free to contact me at alexi.zein@gmail.com.
