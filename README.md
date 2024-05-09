# Credit Risk Classification #
* supervised learning challenge

## Instructions ##
1. Split the Data into Training and Testing Sets
2. Create a Logistic Regression Model with the Original Data
3. Write a Credit Risk Analysis Report

## Analysis ##
The purpose of this analysis is to train and evaluate the accuracy of a dataset from a peer-to-peer lending services company to identify the creditworthuness of borrowers. <br/><br/>

Factors that determined loan status:
* loan_size
* interest_rate
* borrower_income
* debt_to_income
* num_of_accounts
* derogatory_marks
* total_debt

There were a total of 77536 values in the data used to measure accuracy. First, the data was separated into labels (loan_status) and features (all data excluding loan_status). These factors were used to split into training and testing datasets to create a logistic regression model. The logitistic regression model was then used to make predicitions. After gathering the predictions,  it was put into a confusion matrix to compare how many predictions were actual or not. Lastly, a classification report was made to check the accuracy scores of thr precision and recall. <br/>

## Results ##
* Accuracy
    * 99% for the f1-score.
    * The f1-score is the average of the precision of recall, so it provides a balance measurement of the model's performance
* Precision
    * Precision is used when the model predicts positive, it is a true positive.
    * 100% for predicting the true healthy loans correctly
    * 85% for predicting the true high-risk loans correctly
* Recall
    * Recall is used when the model predicts negative, it is actually negative.
    * 99% for predicting the healthy loans correctly
    * 91% for predicting high-risk loans correctly

## Summary ##
This model did well at predicting the creditworthiness of borrowers with an accuracy of 99%. In terms of a company wanting to save money and want borrowers to have a good relationship with loan repayment, limiting the amount of false positives (saying high-risk loans were healthy loans) would be ideal. Since this model has high predictions for the actual healthy loans (100% precision and 99% recall), companies will likely correctly give loans to actual low risk loan borrowers. As for predicting high risk loans, 85% for precision is not bad in terms of finding actual high-risk loans. It would be better to flag more people as high-risk falsely compared to low-risk so companies wouldn't lend so much money out to the wrong people. <br/><br/>

Since this model has a high accuracy, it is recommended for companies that prefer low-risk lending with slight inaccuracies when it comes to high-risk lending. Overall having a higher macro average for recall at 95% compared to precision at 92% this is more ideal at catching all the healhy loans correctly.