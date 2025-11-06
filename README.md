# Will a Bank Client Subscribe a Term Deposit
**Assignment Jupyter Notebook URL Address:** https://github.com/zaboush/Model_17_Assignment_17p1/blob/main/Model_17_Assignment_17p1.ipynb
## Note: I couldn't execute the code using Jupyter notebook due to the limited resources, therefore used Colab instead.
## Project Objectives
The goal of this project is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) we encountered in this section of the program. We will use a dataset related to the marketing of bank products over the telephone.
## Data Description
The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. 
The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).
## Business Objective
The business objective is to predict whether a client will subscribe to a term deposit based on the provided marketing campaign data.
## Data Understanding
**Steps for Data Understanding and Quality Assessment:**  
1. Understanding and analyzing the data: Examined the dataset, identified data types, checked for missing values, and explored unique values in categorical features.
Reading in the data: Loaded the data into a pandas DataFrame.
2. Understanding the features and performing initial data cleaning/feature engineering: Performed data cleaning by removing rows with 'unknown' values and outliers based on age, duration, campaign, previous contacts, education, and default status.
3. Stating the business objective: Defined the goal of predicting client subscription to a term deposit.
4. Engineering features: Applied one-hot encoding to categorical features and scaled the numerical features.

## Key Findings
**Analyzing the plots, several features appear to be key predictors for whether a client will subscribe to a term deposit:**
- **duration:** <font color="blue">This feature shows a significant difference in distribution between 'yes' and 'no' subscribers. Clients who subscribed generally have longer contact durations.
- **poutcome:** <font color="blue">Clients with a 'success' outcome from the previous campaign are much more likely to subscribe in the current campaign.
euribor3m and nr.employed: These economic indicators show noticeable differences in distribution between the two target classes, suggesting their influence on subscription.
- **contact:** <font color="blue">Clients contacted by 'cellular' are more likely to subscribe than those contacted by 'telephone'.
- **month:** <font color="blue">Certain months, like March, September, October, and December, show a higher proportion of subscriptions.
These features exhibit clear variations in distribution based on the target variable 'y', making them potentially strong predictors.
## Modelling and Models Comparison
**Creating models and comparing their performance involved the following steps:**
- Splitting the data: Divided the data into training and testing sets.
- Establishing a baseline model: Calculated the baseline accuracy based on the majority class.
- Building and scoring models: Trained and evaluated Logistic Regression, KNN, Decision Tree, and SVM (with linear kernel) models.
- Model Comparisons: Compared the performance of the models using accuracy, precision, recall, and F1-score on both unscaled and scaled data. Visualized the accuracy comparison of scaled models.
## Recomendation
**Based on the analysis:**
- Accuracy: Logistic Regression and SVM (Linear Kernel) generally showed higher accuracy on both unscaled and scaled data.
- F1-score: KNN (Scaled) achieved the highest F1-score, indicating a good balance between precision and recall for identifying subscriptions.
- Precision: SVM (Linear Kernel, Scaled) and Logistic Regression (Scaled) had the highest precision, useful for minimizing false positives.
- Recall: KNN (Scaled) and Decision Tree (Scaled) generally showed higher recall, useful for identifying more true positives.

For this business case, Logistic Regression seems to be the best suitable model to use.
