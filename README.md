# Santander Customer Satisfaction
This is a self case study based on a [Kaggle competition](https://www.kaggle.com/c/santander-customer-satisfaction?rvi=1).

Customer satisfaction is one of the most important key performance indicators in every company today and is seen as a key element of a company's success. Unhappy customers don't stick around. What's more, unhappy customers rarely voice their dissatisfaction before leaving. Santander is a Spanish multinational corporation bank and financial based company which operates in Europe, North and South America, and also Asia. In this Kaggle competition that is conducted by Santander we need to predict whether a customer is dissatisfied with their services early on based on the features provided by the company. This will help them to take proactive steps to improve the customer satisfaction before the customer leaves.

Here I have removed sparse features, features that had high correlation with each other and also features that had low correlation with dependant variable ("TARGET"). I created 6 datasets (created more than 100 features (at least) for the 6 datasets) and applied ***logistic regression, decision trees, random forest, XGBoost and Lightgbm.*** 


My detailed approach can be viewed in this [medium](https://medium.com/@ashishthomas7/santander-customer-satisfaction-a-self-case-study-using-python-5776d3f8b060?source=friends_link&sk=2fa9b7734bc9a957fedb9e91fec93d7f) article. 

# Results
| Sl No. | Model | Kaggle Public score (AUC) |
| - | --------------------- | ----------- |
| 1. | Ensembling(Average of two best models) | 0.82746 |
| 2. | log re(top 250) xgb | 0.82734 |
| 3. | normal re(top 250) xgb | 0.82713 |
| 4. | Stacking (logistic Regression) | 0.82310 |
| 5. | normal (top 250) xgb | 0.81952 |
| 6. | log ohe xgb | 0.81851 |
| 7. | normal ohe(top 250) xgb | 0.81560 |
| 8. | log xgb | 0.81131 |

Contents of the Code Files are given below :-

| Code File | Description  | 
| ----  | --------- |
| EDA.ipynb    | Exploratory Data Analysis|
| Feature_Engineering.ipynb    | Feature Engineering|
| final.ipynb    | Function 1 - takes input X, returns prediction Y,Function 2 - takes input (X,Y) returns evaluation metric (AUC)|
| Final_ensembling.ipynb    | Final ensembling,stacking models and data interpretation|
| Modelling_LogOHE.ipynb    | Modelling experiments on Log transformed One Hot Encoded Dataset|
| Modelling_Log_RE.ipynb   | Modelling experiments on Log transformed Response Encoded Dataset|
| Modelling_Normal.ipynb  | Modelling experiments on Normal Dataset|
| Modelling_Normal_OHE.ipynb   | Modelling experiments on Normal One Hot Encoded Dataset|
| Modelling_Normal_RE.ipynb   | Modelling experiments on Normal Response Encoded Dataset|
| modelling_logTransformed.ipynb  | Modelling experiments on Log Transformed Dataset|
