# credit-risk-classification

## Overview of the Analysis

The analysis of this machine learning is to accurately identify good loans and high risk loans given a dataset comprised of fields such as: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt. There is an additional field, loan status, that serves as the labels for the supervised machine learning. This field is the actual mark for whether the loan is good or bad. This is also the column that we are trying to predict.

The machine learning I did on this dataset cam in stages. We started by importing the data into a pandas dataframe to make it easier to work with. We then split the data into a training set and a testing set. This split is done on a random subset of the total data. We then created a logistical regression model using the training data, fit the model, and then made predictions using the model. Finally, we evaluated the accuracy, precision, and recall of the model by comparing our predictions with the labels (aka answers). We generated a Confusion Matrix and a Classification Report to help evaluate the reliability of the model we created.

## Results

Machine Learning Model 1: Logistical Regression Model
    * Description of Model 1: This model estimates the probability of an event occurring. This model is better at estimating relationships between variables when there are a lot of independent variables.
    * Accuracy: 0.99
    * Precision: for good loans - 1.00, for high risk loans - 0.89
    * Recall: for good loans - 1.00, for high risk loans - 0.87

## Summary

There was only one model created here using the traingin data and tested on the test data. I would recommend this model as it scored pretty highly in terms of accuracy, precision, and recall across the board. This model definitely did a better job at estimating 0's than 1's (good loans than high risk loans). I believe it is important to accurately estimate good loans, but I believe it's okay to be a bit more inconsistent on high risk loans. High risk loans should be evaluated by a human anyway, so if this model gets it right 90% of the time that feels good to me.
