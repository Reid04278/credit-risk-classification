# Module 20 Report

##  Overview of the Analysis
The purpose of this analysis was to build a regression model. We were given lending data and the goal was to predict the creditworthiness of loan borrowers.
We predicted people's creditworthiness by splitting our data into X and y values to create our labels. The y variable came from the loan_status column in the dataframe and the X variable
came from the other columns in the dataframe. This created two labels 0 and 1. 0 means the loan is healthy. 1 means the loan has a very high risk of defaulting.
Once we split our data into testing and training set, we fit the training data into a Logistic Regression model. Then I made predictions on the test data and created a dataframe showing
the results. Next, we calculated the balanced accuracy score, confusion matrix and created the classification report. For the second part, I created a second Logistic Regression model by 
using resampled data by using the RandomOverSampler method from the imbalanced-learn library. I resampled the data and did similar steps as above.



##  Results
* Machine Model 1:
* 0: Precision 1.00, Recall 1.00, f1-score 1.00
* 1: Precision 0.87, Recall 0.89, f1-score 0.88


* Machine Model 2:
* 0: Precision 0.99, Recall 0.99, f1-score 0.99
* 1: Precision 0.99, Recall 0.99, f1-score 0.99




  ## Summary
  According to the classification reports. Both models would be sufficient to use in determining creditworthiness of loan borrowers. If I were to recommend a model. I would
  recommend model 2. The reason being that the stats for precision, recall and the f1-score are near perfect in predicing both the 0 and 1 labels.
  Machine Model 1 is great if someone wanted to predict just the 0 label but it needs a little more work to predict the 1 label. 
