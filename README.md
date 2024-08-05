# Module_20_Challenge
Baileys UWA Submission for Module 20 challenge



## Overview of the Analysis
The purpose of this analysis was to evaluate the performance of a logistic regression model in predicting loan statuses, specifically distinguishing between healthy loans (0) and high-risk loans (1). The dataset contains financial information related to various loans, and our objective was to predict the loan_status based on the provided features.

### The key variable we aimed to predict was the loan_status:

0: Healthy loan
1: High-risk loan
### The distribution of loan_status in the dataset is as follows:

Healthy loans (0): 15001 instances
High-risk loans (1): 507 instances
### The machine learning process involved the following stages:

* Data Preparation: Splitting the data into features (X) and labels (y).
* Data Splitting: Using train_test_split to divide the data into training and testing sets.
* Model Training: Fitting a logistic regression model on the training data (X_train and y_train), with a specified random_state of 1.
* Model Evaluation: Generating predictions on the testing data (X_test), and evaluating the model's performance using a confusion matrix and classification report.
* The primary method used was LogisticRegression from the sklearn.linear_model module.

## Results
* Logistic Regression Model:
    * Accuracy Score: 99%
* Precision Score:
    * Healthy loans (0): 1.00
    * High-risk loans (1): 0.86
* Recall Score:
    * Healthy loans (0): 0.99
    * High-risk loans (1): 0.94
## Summary
The logistic regression model demonstrates excellent performance in predicting loan statuses. Key metrics are as follows:

Healthy Loans (0): The model achieved perfect precision (1.00) and near-perfect recall (0.99), indicating that almost all loans identified as healthy were indeed healthy, and nearly all actual healthy loans were correctly identified.
High-Risk Loans (1): The model achieved strong precision (0.86) and very high recall (0.94), meaning that 86% of loans predicted to be high-risk were actually high-risk, and 94% of actual high-risk loans were correctly identified.
Given its high accuracy, precision, and recall scores, I recommend using this logistic regression model for loan risk assessment. It provides a reliable method for identifying high-risk loans, which can significantly aid the company's risk management strategy. The model's balanced performance across both classes makes it a robust choice for this classification task.