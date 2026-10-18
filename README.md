# Breast Cancer Diagnostic Data Analysis

## Overview
This project explores how cell measurements differ between benign and malignant breast tissue samples, and tests whether a simple model can tell them apart. It uses the Wisconsin Breast Cancer Diagnostic dataset from the UCI Machine Learning Repository.

## What I did
- Loaded and inspected the dataset (569 samples, 30 measurements)
- Checked for missing values and duplicates (none found)
- Visualised how radius, area, texture and concavity differ between benign and malignant samples
- Trained a logistic regression model on scaled data
- Evaluated it with a confusion matrix, sensitivity (recall) and specificity

## Key results
| Metric | Result |
|---|---|
| Accuracy | 98.25% |
| Sensitivity (malignant cases caught) | 97.6% (41 of 42) |
| Specificity (benign cases cleared) | 98.6% (71 of 72) |

## Key findings
- Malignant samples tended to have larger and more irregular cell nuclei than benign ones.
- Radius, area and concavity separated the two groups most clearly; texture overlapped more.
- The model missed one malignant sample, the more serious kind of error in a diagnostic setting.

## Limitations
Small dataset, one model and one train-test split, and related measurements make it hard to rank individual features. This is a learning project and not a clinical diagnostic tool.

## Tools used
Python, pandas, matplotlib, seaborn, scikit-learn, Google Colab

## Notebook
See `Breast_Cancer_Diagnostic_Analysis.ipynb` for the full analysis.
