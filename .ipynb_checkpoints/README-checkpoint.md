# Loan Risk Prediction with Logistic Regression

## Overview

This project focuses on predicting loan risk by classifying loans as either high-risk (1) or healthy (0) using machine learning techniques. Specifically, logistic regression was applied to a dataset that contains various financial and personal features about loans. The goal is to identify high-risk loans with high accuracy, ensuring that those loans are flagged for further review.

The project consists of data preprocessing, model training, evaluation, and analysis to predict whether a loan is high-risk or healthy. The primary evaluation metrics for the model are accuracy, precision, and recall, with a focus on recall for high-risk loans due to the importance of identifying them accurately.

### Data

The dataset used in this project is stored in the lending_data.csv file and contains information related to loans, such as financial data and loan status. The target variable, loan_status, indicates whether the loan is high-risk (1) or healthy (0).

Key features include:

Financial indicators (e.g., income, loan amount, term, etc.)
Personal information about borrowers (e.g., credit score, marital status, etc.)

### Methodology

1. Data Preprocessing
Loaded the dataset into a Pandas DataFrame.
Reviewed the dataset and performed basic cleaning, if necessary.
Separated the features (X) and labels (y) for machine learning.
Split the data into training and testing sets using train_test_split from scikit-learn.
Scaled the feature data using StandardScaler to normalize the values.
2. Model Building
Used the logistic regression model from sklearn.linear_model to build the classifier.
The model was trained on the scaled training data and evaluated using the testing data.
3. Evaluation Metrics
Accuracy, precision, and recall were calculated for both the healthy loans (0) and high-risk loans (1).
The confusion matrix, classification report, and accuracy score were generated to assess model performance.
4. Model Performance
Accuracy: 99%
Precision (Healthy Loan): 1.00
Recall (Healthy Loan): 0.99
Precision (High-Risk Loan): 0.84
Recall (High-Risk Loan): 0.94

Given the context of loan risk prediction, the model's recall for high-risk loans is the most critical metric. The model's performance in accurately identifying high-risk loans (recall of 0.94) is an important factor in minimizing financial loss due to misclassification.