# Module 12 Report Template

## Table of Contents:

Overview of the Analysis
Model Results
Summary

# Overview of the Analysis

Lending companies lend money/properties to borrowers with the expectation that the borrower will either return the asset or repay the lender. Credit Risk is associated with a borrower not returning an asset or paying a loan back causing a lender to lose money. This is measured by lenders in many ways, however in this analysis we will use Machine Learning to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Using a machine learning model, we will try to determine which loans are healthy (low-risk) or non-healthy (high-risk) based on the loan status provided by the lending company. The Logistic Regression Algorithm is the best tool to use for our machine learning model since it is widely used to predict the probability of a target variable in classification problems.

# Model Results

Using the dataset provided by the lending company, a Logistic Regression Model was created that generated an accuracy score of 99% for the oversampled dataset. The model's recall value for non-healthy loans is 94% and for healthy loans is 99%, indicating that the model predicts loan statuses as healthy better than being able to predict loan statuses as non-healthy due to the dataset being imbalanced.

# Confusion Matrix - Oversampled Dataset

True Negatives (TN): 18655 (Actual Healthy Loans correctly predicted as Healthy)
False Positives (FP): 110 (Actual Healthy Loans incorrectly predicted as Non-Healthy)
False Negatives (FN): 36 (Actual Non-Healthy Loans incorrectly predicted as Healthy)
True Positives (TP): 583 (Actual Non-Healthy Loans correctly predicted as Non-Healthy)

# Classification Report - Oversampled Dataset

Precision for Healthy Loans: 1.00
Recall for Healthy Loans: 0.99
Precision for Non-Healthy Loans: 0.84
Recall for Non-Healthy Loans: 0.94
F1 Score for Healthy Loans: 1.00
F1 Score for Non-Healthy Loans: 0.89
Average Precision: 0.99
Average Recall: 0.99
Average F1 Score: 0.99

# Summary

The Logistic Regression model fitted with oversampled data performed much better than the model fitted with imbalanced data due to the data being balanced, resulting in a higher accuracy score and improved recall for non-healthy loans. The lending company would likely prefer fewer False Positives due to the high possibility of losing funds when classifying non-healthy loans as healthy.

Based on this analysis, it is recommended to use the Logistic Regression Model fitted with balanced (oversampled) data for classifying healthy and non-healthy loans.

