# Module 12 Report Template

## Overview of the Analysis

In this analysis, I built a machine learning model to predict whether a loan is healthy (0) or high-risk (1). The goal was to identify high-risk loans accurately, so the model can be used to better assess financial risk in loan portfolios.

The dataset included various features about loans, such as financial and personal information, with the target variable being loan_status (1 for high-risk loans and 0 for healthy loans). I used a logistic regression model to predict the risk level based on these features.

The analysis involved several stages:

Data Preprocessing: I began by cleaning the data, splitting it into training and testing sets, and scaling the feature values.
Model Selection: I chose the logistic regression model due to its simplicity and efficiency in binary classification tasks.
Model Evaluation: I evaluated the model's performance using a confusion matrix, precision, recall, and the classification report.

## Results

Logistic Regression Model:
Accuracy: 99%
Precision (Healthy Loan): 1.00
Recall (Healthy Loan): 0.99
Precision (High-Risk Loan): 0.84
Recall (High-Risk Loan): 0.94

## Summary

The logistic regression model performs very well overall, with high accuracy and precision for healthy loans. However, recall for high-risk loans is more important, as we aim to minimize the number of high-risk loans missed by the model. The model's recall for high-risk loans (0.94) is quite strong, indicating it is effective at identifying those loans.

Given that predicting high-risk loans is crucial in minimizing financial loss, the logistic regression model appears to be a good choice. Its relatively high recall for the high-risk class suggests it can be relied on to identify most of the risky loans, which is important for loan management and risk mitigation.

If needed, further tuning or testing of more advanced models like Random Forest or XGBoost could be explored, but the logistic regression model offers a solid baseline for this problem.