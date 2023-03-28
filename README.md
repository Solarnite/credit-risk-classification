## credit-risk-classification
 
# Overview of the Analysis

The purpose of this analysis is to create a logistic regression model to predict whether a loan is high-risk or healthy based on various factors such as loan size, interest rate, borrower income, debt-to-income ratio, and etc. It was also conducted to compare the strengths of two different models and analyze the results. This will help the company make informed decisions about which loans to approve or reject.

**Dataset**

Total records: 77536
- Healthy Loans: 75036, High-Risk: 2500

# Results
**Machine Learning Model 1 (Logistic Regression Model with the Original Data):**
- Balanced Accuracy 
  - 95%
  
- Precision
  - Healthy Loan: 100%
  - High-Risk Loan: 85%
  
- Recall
  - Healthy Loan: 91% 
  - High-Risk Loan: 91%

**Machine Learning Model 2 (Logistic Regression Model with Resampled Training Data):**
- Balanced Accuracy
  - 99%
  
- Precision: 
  - Healthy Loan: 100%
  - High-Risk Loan: 84%
  
- Recall
  - Healthy Loan: 99% 
  - High-Risk Loan: 99%
 
# Summary
 
**Logistic Regression Model with original data**

For healthy loans ('0') the logistic regression model has  very precise predictions with 100% correct predictions. The recall was 99% which classified the vast majority of the possible healthy loans as 'healthy loans', however not every single one. With the f1 score being 100% and a balanced accuracy score of 95% it is still a great model for predicting the status of the healthy loans.

For high-risk loans ('1') the model was correct for predictions 85% of the time, with a recall score of 91% and an f1 score of 88% which is possible that the classification of some of the loans being 'high-risk' may be false positives and not actually high-risk. The model performed well enough for high-risk loans. 

**Logistic Regression Model with resampled data**

Similar to the previous model, the oversampled model was correct for predictions of healthy loans ('0') 100% of the time with a recall score of 0.99% and an f1 score of 100%. This model did a great job at predicting the status of the healthy loans.

For high-risk loans ('1') the oversampled model had precision of 85% with a higher recall score of 99% and an f1 score of 91%.The balanced accuracy score was 99% and the macro avg for the recall and f1 score are higher with this model from the classification report than from the previous model with the original data. 

**Overall**

The model may not be considered very good, however it can be taken to be good. Judging by the recall scores for high-risk loans the second model had a higher recall which was 99%. A credit company might want a model that has a higher recall as the prediction of high-risk loans is more important than healthy loans.
  
