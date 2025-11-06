# Will a Bank Client Subscribe a Term Deposit
Comparing Classifiers to predict if Portuguese banks clients will subscribe a term deposit 
**Assignment Jupyter Notebook URL Address:** https://github.com/zaboush/Model_11_Assignment_11p1/blob/main/prompt_II_091725.ipynb
## Project Objectives
The goal of this project is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) we encountered in this section of the program. We will use a dataset related to the marketing of bank products over the telephone.
## Data Description
The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. 
The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).
## Problem Statement
The goal is to understand what factors make a car more or less expensive. As a result of our analysis, we should provide clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car.
Todo that, we need to explore the data provided using our knowledge of plotting, statistical summaries, and visualization using Python. Then use various linear regression models and evaluate then to understand how each car feature contribute to the rice. We then publish our findings in a public facing github repository alongside Pthon code used to analyse the data and conclusions drawn.
## Data Understanding
**Steps for Data Understanding and Quality Assessment:**  
1. Load the dataset and display the first few rows to get a sense of the data structure and content.

## Key Findings
**Based on our analysis and the Lasso model, the following features were found to be the most significant drivers of used car prices:**
- Vehicle Age and Odometer Reading: As expected, older cars with higher mileage tend to have lower prices. These are strong negative predictors of price.

## Recomendation
**Based on the analysis:**
Accuracy: Logistic Regression and SVM (Linear Kernel) generally showed higher accuracy on both unscaled and scaled data.
F1-score: KNN (Scaled) achieved the highest F1-score, indicating a good balance between precision and recall for identifying subscriptions.
Precision: SVM (Linear Kernel, Scaled) and Logistic Regression (Scaled) had the highest precision, useful for minimizing false positives.
Recall: KNN (Scaled) and Decision Tree (Scaled) generally showed higher recall, useful for identifying more true positives.
