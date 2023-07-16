# Module 20 Report

##  Overview of the Analysis
The purpose of this analysis was to build a regression model using lending data to predict the creditworthiness of loan borrowers.
I predicted borrowers' creditworthiness by splitting the lending data into X and y values to create the following labels: the y variable was assigned to the loan_status column in the dataframe and the X variable was assigned to all the other columns in the dataframe. This created two labels, 0 and 1. The label "0" indicates the loan is healthy. The label "1" indicates the loan has a very high risk of defaulting.
I split the data into testing and training sets and then fit the training data into a Logistic Regression model.  I then made predictions on the test data and created a dataframe showing
the results. Finally, I calculated the balanced accuracy score, confusion matrix and created the classification report. 

For the second part of this assignment,  I created a second Logistic Regression model using the RandomOverSampler method from the imbalanced-learn library. I resampled the data, made predictions, and calculated scores as described above.



##  Results
* Machine Model 1:
* 0: Precision: 1.00, Recall: 1.00, balanced accuracy score: 0.944, f1-score: 1.00
* 1: Precision: 0.87, Recall: 0.89, balanced accuracy score: 0.944, f1-score: 0.88


* Machine Model 2:
* 0: Precision: 0.99, Recall: 0.99, balanced accuracy score: 0.994, f1-score: 0.99
* 1: Precision: 0.99, Recall: 0.99, balanced accuracy score: 0.994, f1-score: 0.99




  ## Summary
Based on the classification reports, both models would be appropriate tools to determine the health of loans. Model 1 was more likely to include false negatives in determining recall.  Model 2 however, was clearly superior in determining the risk of loan default, as well as being an equally good predictor of the healthiness of loans as Model 1. Therefore, I recommend the use of Model 2 to determine the creditworthiness of loan borreowers. 
