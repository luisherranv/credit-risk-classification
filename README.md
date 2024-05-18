# Log Regression Model Challenge
A log regression model was used in this project to predict based on the following variables (loan_size	interest_rate	borrower_income	debt_to_income	num_of_accounts	derogatory_marks	total_debt) if a loan is a "healthy loan" (0) or a "high-risk loan" (1). After training and fitting the model, the resuts of the confusion matrix are as follows:

## Confusion Matrix
True Healthy Loan Predictions: 18652
False High-Risk Loan Preictions: 113
False Healthy Loan Predictions: 10
True High-Risk Loan Preictions: 609

## Classification Report
The results of the classification report are shown below:

<img width="464" alt="image" src="https://github.com/luisherranv/credit-risk-classification/assets/150373234/c730f74b-d9ed-4aed-9cfa-8e60265942c0">

### Precision:
Healthy Loan: 100%
High-Risk Loan: 84%

Overall the model is relatively precise in predicting wether a loan is heatlhy or high risk. There is a relatively lower precision (0.84) for predicting if the loan is high-risk, compared to almost full certainty (1.0) that the loan is healthy. This means that the model predicitons for a healthy loan were 100% precise as tested by the test data, but only 84% of the predictions for the high-risk loan were correct. 

### Recall
Healthy Loan: 98%
High-Risk Loan:99%

Overall the model has relatively high recall for both predictions, nearly 100%. This shows that the model was capable of accurately predicting the the true positive cases for both types of loans.

### f1 Score

Healthy Loan: 100%
High-Risk Loan:91%
Overall: 99%

The model has very satisfactory f1 scores for each of the loan predictions which take into account both the importance of precision and recall. The model appears to be ideal for predicting instances of heatlhy loans, however the high-risk loan requires a bit of improvement. This is understandable since the dataset is highly skewed for the number of healthy loans, meaning more training data might be required that include higher instances of high risk loans, or more variables. However, the overall accuracy f1 score is 99% for the entire model, which shows high confidence for using it to make predictions. 
