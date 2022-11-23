# Credit Risk Analysis

## Overview of the Analysis

The purpose of this analysis was to determine credit risk for a large number of loans. The given data is form LendingClub, a peer-to-peer lending services company. The dataset includes information about credit card holders as well as information about their credit statements.

The analysis includes six supervised machine learning models and evaluates each model's performance. The overall goal of this analysis is to determine if any of these models can be used to predict if a loan is high or low risk accurately and efficiently. 

## Results

### Naive Random Oversampling
* Balanced Accuracy Score: 0.65
* High Risk Precision: 0.1
* Low Risk Precision: 1
* High Risk Recall: 0.73
* Low Risk Recall: 0.58

### SMOTE Oversampling
* Balanced Accuracy Score: 0.66
* High Risk Precision: 0.1
* Low Risk Precision: 1
* High Risk Recall: 0.63
* Low Risk Recall: 0.69

### Undersampling
*Balanced Accuracy Score: 0.54
*High Risk Precision: 0.1
*Low Risk Precision: 1
*High Risk Recall: 0.69
*Low Risk Recall: 0.40

### Combination Sampling
* Balanced Accuracy Score: 0.64
* High Risk Precision: 0.1
* Low Risk Precision: 1
* High Risk Recall: 0.70
* Low Risk Recall: 0.58

### Balanced Random Forest Classifier
* Balanced Accuracy Score: 0.79
* High Risk Precision: 0.3
* Low Risk Precision: 1
* High Risk Recall: 0.70
* Low Risk Recall: 0.87

### Easy Ensemble AdaBoost Classifier
* Balanced Accuracy Score: 0.93
* High Risk Precision: 0.9
* Low Risk Precision: 1
* High Risk Recall: 0.92
* Low Risk Recall: 0.94

## Summary

All machine learning models are not sufficient for any real application. This is shown in the high risk precision values. The highest "high risk precision" value is 0.9, in the Easy Ensemble AdaBoost Classifier model. This means that 9% of all loan applications that were flagged as "high risk" are actually high risk, and the remaining 91% are actually low risk.

Looking at the individual recall values, it would be assumed that 0.92 for high risk recall in the same Easy Ensemble AdaBoost model is sufficient. Because recall is not enough for machine learning models to be sufficient, the other factors including precision and f1 score, prove that this model is not sufficient for real world application.

Additionally, since all other models have lower precision, recall, f1 values and balanced accuracy scores than the Easy Ensemble AdaBoost Classifier, it is understood that none of the models are sufficient for real world application. 
