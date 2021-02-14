# Credit_Risk_Analysis

## Overview of the Analysis:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we have used different techniques to train and evaluate models with unbalanced classes and used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Results:

### The balanced accuracy scores and the precision and recall scores of all six machine learning models. 

For any machine learning model, we first start with converting our string values into numerical ones and spliting the data into training and testing. We have used 6 different machine learning models here as follows;

- Naive Random Oversampling
  - Balanced Accuracy score - 0.6497536370265621

  <img src="/Images/Naive_Random_Oversampling.png" width="400"/> 

- SMOTE Oversampling
  - Balanced Accuracy score - 0.6443721269403855

  <img src="/Images/SMOTE_Oversampling.png" width="400"/> 

- Undersampling
  - Balanced Accuracy score - 0.6443721269403855

  <img src="/Images/Undersampling.png" width="400"/> 

- Combination (Over and Under) Sampling
  - Balanced Accuracy score - 0.5172544730088513

  <img src="/Images/Combination_sampling.png" width="400"/> 

- Balanced Random Forest Classifier
  - Balanced Accuracy score - 0.7877672625306695

  <img src="/Images/Random_Forest.png" width="400"/> 

- Easy Ensemble AdaBoost Classifier
  - Balanced Accuracy score - 0.925427358175101

  <img src="/Images/AdaBoost.png" width="400"/> 


## Summary: 

Balanced Accuracy is the average of sensitivity and specificity with a min = 0 and max = 1. Balanced accuracy is the most accurate the closer its value is to 1. From the 6 machine learning models we worked with in this challenge, Easy Ensemble AdaBoost Classifier has the highest balanced accuracy score at 0.925427358175101

f1 score tells us what percent of positive predictions were correct? If we look at the f1 score for all 6 models above we will see that the f1 score for Easy Ensemble AdaBoost Classifier is the higest as well at 0.97. f1 score is a weighted harmonic mean of precision and recall such that the best score is 1.0 and the worst is 0.0. 

We can therfore recommend using the Easy Ensemble AdaBoost Classifier model for our data.