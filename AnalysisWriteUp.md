# credit-risk-classification
# Module 12 Report/Analysis

Background
  The purpose of this analysis was to use various techniques to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company. In doing so, I was able to build a model that can identify the creditworthiness of borrowers. 


Financial Information
  The financial dataset given was comprised of 77,536 data points. After obtaining and reviewing the data, it was decidedly best to split the set into both a testing and a training set. 


Predicted Values
  The  x-value, or independent variable, was represented by the following metrics: loan size, interest rate, borrower income, debt to income ratio, number of accounts and derogatory marks. The y-value, or dependant variable, was the "loan status." This value represents the health of the loan--if a loan is healthy or at risk. It was important to note that a value of 0 in the “loan_status” column meant that the loan is healthy, while a value of 1 meant that the loan has a high risk of defaulting.


Machine Learning Stages
  After splitting the data, I was able to fit a logistic regression model by using the training data (X_train and y_train). I then saved the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model. After this, I evaluated the model’s performance by generating a confusion matrix and printing the classification report.


Methods Utilized
  Using the original data, I created a Logostic Regression Model. Using the training data to eliminate data imbalances, I created a Logistic Regression Model with Resampled Data. 

## Results
* Machine Learning Model 1: Original Data
  * Balanced Accuracy Score: 99%
  * Precision Score: 
        * healthy loans: 100% precise predictions
        * high risk loans: 87% precise predictions
  * Recall Score: 
        * healthy loans: 100% recall predictions
        * high risk loans: 89% recall predictions


* Machine Learning Model 2: Resampled Data
  * Balanced Accuracy Score: 100%
  * Precision Score: 
        * healthy loans: 100% precise predictions
        * high risk loans: 87% precise predictions
  * Recall Score: 
        * healthy loans: 100% recall predictions
        * high risk loans: 100% recall predictions

## Summary
Reccomendation:
I would recommend using Model 2 to drive analysis. While both were quite similar in their balanced accuracy scores and the precision and recall scores, Model 2 did show to have a higher balanced accuracy score by 1% as well as a better ability to recall predictions in higher risk loans. 
In this instance, it was beneficial to predict both health and high risk loans so that we could get a more wholistic view of the viability of both models.
