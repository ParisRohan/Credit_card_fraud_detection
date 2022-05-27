# Credit_card_fraud_detection
A supervised ML binary classification model built on an imbalanced dataset to detect if a transaction is fraudulent or not.

# Workflow

## 1. Data Collection and Description
* The dataset is donwloaded from Kaggle:-
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?datasetId=310&sortBy=dateRun&tab=profile
* The dataset contains transactions made by credit cards in September 2013 by European cardholders in a span of two days.
* The dataset contains 284807 rows and 31 columns
* Feature Description:
  * Time: Number of seconds elapsed between this transaction and the first transaction in the dataset
  * V1 to V28: Sensitive data masked using PCA
  * Amount: Transaction amount
  * Class: 1 for fraudulent transactions, 0 otherwise -> TARGET feature
* Target feature distribution -> The number of non-fraudulent transactions is 284315 and the number of fraudulent transactions is 492
![image](https://user-images.githubusercontent.com/49038495/170679041-d3c1a3a2-0b25-438d-abd4-76ab92a95cf0.png)

## 2. Model Building
* The imbalanced dataset is treated using SMOTE technique to balance the number of records in the Target feature
![image](https://user-images.githubusercontent.com/49038495/170679481-d40dcceb-3c8a-4530-bb85-8ef6b0369a0f.png)
* Logistic Regression performance metrics:
![image](https://user-images.githubusercontent.com/49038495/170679626-5af04467-c6b3-4111-870b-6641a6d05cc2.png)
* XGBoost model performance metrics:
![image](https://user-images.githubusercontent.com/49038495/170679719-ff10a849-ae75-41eb-b867-f31958c06634.png)
