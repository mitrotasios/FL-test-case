# Testing the application of Federated Learning on Fraud Detection
The purpose of the following Notebook it to test the possible application of Federated Learning to insurance fraud cases regarding claims.

View the Notebook Directly: https://nbviewer.jupyter.org/github/mitrotasios/FL-test-case/blob/main/test_cc_fraud.ipynb

## Test Design and Hypothesis
In order to test the possibility of applying a Federated Learning approach to insurance fraud, a public dataset with credit card transactions is used, where samples are classified into fraudulent and non-fraudulent transactions. The data consists of highly imbalanced financial data and can therefore be used as a comparison to claims use cases in insurance.

The machine learning models which are primarily used in this analysis are:

- XGBoost (Extreme Gradient Boosting)
- Random Forest
- Logistic Regression

The models are evaluated using the ROC-AUC score, testing the models' separability, i.e. their ability to distinguish between the positive class (fraud) and negative class (not fraud).

The underlying hypothesis is that, if Federated Learning can be applied to such a case, then the accuracy of models trained on a smaller subset of the whole dataset is substantially lower than the overall accuracy of models trained on the complete dataset. Assuming that this is the case, it would imply that there is an incentive for insurers lacking the required resources, i.e. training data, to build a sufficiently accurate model.
