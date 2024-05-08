# credit-risk-classification
Data Analytics Bootcamp Module 20 Challenge


## Overview of the Analysis

With the historical lending activity from a peer-to-peer lending services company, I used a logistical regression model to help identify the creditworthiness of borrowers. The size of the loan, interest rate, borrower income, debt-to-income, number of accounts, derogatory marks, and total debt were all used to help predict the risk level of a loan.

In order to create the logical regression model, I had to split the data into training and testing sets. After fitting the training data to the model I saved the predictions on the testing data. Finally, I evaluated the model with a confusion matrix and classification report. At first I used the L-BFGS solver but after testing the other solvers, settled on the Newton Cholesky solver.


## Results

Classification scores for high-risk loans:
* Accuracy Score - 99%
    * Even though the accuracy is near perfect, it is almost too good to trust. This is evident when the f1 score for high-risk loans is down to 89%.
* Precision Score - 85%
    * Out of all the borrowers that the model predicted would be high-risk, 85% actually were. 
* Recall Score - 93%
    * Out of all the borrowers that ended up being high-risk, the model made correct predictions 93% of the time.


## Summary

To minimize the risk to the lending company, it's important to focus on the accuracy of the model to correctly identify and avoid high-risk loans. Because it would be dtrimental to the lending company to have too many high-risk loans, we don't want too many false negatives. This is why a recall score of 93 is important to look at in addition to the accuracy and precision scores. Therefore, I would say that the lending company can rely on the model.