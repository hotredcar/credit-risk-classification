# Module 12 Credit Risk Analysis Report

## Overview of the Analysis

In this analysis, we aimed to develop a machine learning model to predict loan defaults based on financial information. The purpose of the analysis was to create a model that could assist in identifying high-risk loans, which would help lenders make more informed decisions and mitigate potential financial losses.

The dataset provided contained various financial features such as:
* loan size
* interest rate 
* borrower income 
* debt to income
* number of accounts 
* derogaratory marks
* total debt

 The target variable we aimed to predict was whether a loan would default (1) or not (0), specifically:
 * loan status 

Before modeling, we conducted exploratory data analysis to understand the distribution of the target variable and features. Then, we split the dataset into training and testing sets.

For modeling, we employed Logistic Regression. After training the model on the training data, we utilized it to predict the labels for the test data. Subsequently, we evaluated the model's performance on the test data by generating a confusion matrix and computing accuracy, precision, and recall scores.

## Results

* Logistic Regression 
    * Accuracy: 0.99
    * Precision for label 0 (healthy loan): 1.0
    * Precision for label 1 (high-risk loan): 0.85
    * Recall for label 0 (healthy loan): 0.99
    * Recall for label 1 (high-risk loan): 0.91
   
## Summary

In summary, the logistic regression model demonstrates strong performance in predicting both healthy and high-risk loans. It achieves high precision and recall for healthy loans, indicating accurate identification of the vast majority of actual healthy loans. While precision and recall are slightly lower for high-risk loans, they still indicate reliable identification.

Overall, the model exhibits high accuracy and performs well for both classes, making it a suitable choice for the task at hand. Its interpretability is valuable for understanding feature impact on loan predictions. More complex models like decision trees or random forests may not be necessary given the logistic regression model's success, but scaling could potentially enhance performance, especially considering the massive range difference in the dataset's features.

The importance of correctly predicting each class (healthy and high-risk loans) varies based on specific objectives. Balancing precision and recall for both classes is crucial for effective model development, ensuring it addresses the goals and constraints of the problem. Achieving this balance ensures that the model accurately identifies both healthy and high-risk loans while minimizing false positives and false negatives, aligning with the objectives of the lending institution or decision-maker.
