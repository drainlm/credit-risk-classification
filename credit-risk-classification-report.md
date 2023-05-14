# Credit Risk Classification Report

## Overview of the Analysis

The purpose of this analysis is to predict the classification of high-risk and healthy loans. The financial data includes rows of information for various borrowers, and columns that contain the size of the requested loan, interest rate, borrower income, debt to income ratio, number of accounts, number of derogatory marks, total debt, and loan status. The loan status variable is used as the target variable with healthy loans being represented by '0' and high-risk loans being represented by '1'. 

The data was heavily imbalanced with 75.036 healthy loans and only 2500 high-risk loans. The Logistic Regression method was used with the original data and then again with OverSampled data, which was used to correct for the imbalance in the data.

## Results

* Logistic Regression Model with Original Data:

  * Balanced Accuracy Score: 95.20%
  * Precision for Healthy Loans: 100%
  * Precision for High-Risk Loans: 85%
  * Recall for Healthy Loans: 99%
  * Recall for High-Risk Loans: 91%
  * False Negatives for Healthy Loans: 102
  * False Negatives for High-Risk Loans: 56
* Logistic Regression Model with OverSampled data:

  * Balanced Accuracy Score: 99.37%
  * Precision for Healthy Loans: 100%
  * Precision for High-Risk Loans: 84%
  * Recall for Healthy Loans: 99%
  * Recall for High-Risk Loans: 99%
  * False Negatives for Healthy Loans: 116
  * False Negatives for High-Risk Loans: 4

## Summary

Both models performed well in predicting healthy loans, due to the large number of healthy loans in the dataset. Due to the imbalance in the dataset, the model trained on oversampled data reduced false negatives for high-risk loans. I would recommend the model using oversampled data as it reduces the risk of inaccurately categorizing a loan as healthy to a high-risk borrower who may default on the loan.
