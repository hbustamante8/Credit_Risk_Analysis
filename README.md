# Credit_Risk_Analysis

## Overview of the Analysis

Fast Lending, a peer-to-peer lending services company wants to use machine learning to predict credit risk. As a data scientist, the purpose of this project is to build and evaluate several machine learning models to predict credit risk using Python to aid Fast. After evaluating each model, a recommendation will be provided to Fast Lending on which model is the best fit to predict credit risk.

Resources used:
* Data Source: LoanStats_2019Q1
* Software used: Jupyter Notebook, Python 3.7, Anaconda Navigator 2.1.1


## Results of all Machine Learning Models

### RandomOverSampler model

![image](https://user-images.githubusercontent.com/96553992/167510525-ac6c2fc1-8a2f-429d-8bee-06475dd8bd82.png)

* The accuracy score for the model is 65%.
* The high risk precision is about 1% and only 62% sensitivity which makes a F1 score of 2%.
* The high number of low risk population, its precision almost 100% with a sensitivity score 68%.

SMOTE Model

![image](https://user-images.githubusercontent.com/96553992/167732926-deedc72e-7b2e-4e49-a8cd-d43629913f67.png)

* The results are fairly similar to the previous model.
* The balanced accuracy score is 62%.
* The high_risk precision is about 1% with about 61% sensitivity.
* As a result of the high number of low_risk population, the precision is almost 100% with a sensitivity of 64%.

ClusterCentroids Model

![image](https://user-images.githubusercontent.com/96553992/167737587-c0e43a49-dac2-4743-aa6c-7dc36c9dcb57.png)

* In this model, the accuracy score is lower compared to previous models at 51%.
* The high_risk precision continues to be at about 1% with an F1 score around 1%.
* The high number of false positives leads to a low sensitivity risk of 44%.


SMOTEENN Model

![image](https://user-images.githubusercontent.com/96553992/167738819-a8f0e95a-fb7a-4358-b107-1ca7f69657c4.png)

* The accuracy score for this model is 65%.
* The high_risk precision is still about 1% while the sensitivity is 69%. Thus, results in an F1 score of only 2%.
* The low_risk sensitivity is a low 62%.

BalancedRandomForest Classifier Model

![image](https://user-images.githubusercontent.com/96553992/167740200-b6bb3bc0-b742-4898-97c6-3b19a44a7f3e.png)

* The accuracy of the model is the higher than the previous mentioned at 79%.
* The high_risk precision continues to be low at 4%  with 67% sensitivity which leads to an F1 score of 7%.
* The low_risk sensitivity is 91% with 100% precision. This is due to the low number of false positives.

EasyEnsembleClassifier model

![image](https://user-images.githubusercontent.com/96553992/167740960-8692d0c0-7e48-4fe1-8cc4-0a61224797bd.png)

* The accuracy score is the highest out of all the model at 93%.
* The high_risk precision is still low at 7% but has a 91% sensitivity leading to a F1 score of 14%.
* Low_risk sensitivity is at 94% and 100% precision. This primarily is because of the low number of false positives in this model.


Summary

Through all the models used to perform credit risk analysis, there was weak precision in determining if credit risk is high. The Ensemble models improved the sensitivity of the high_risk substantially. Specifically, the EasyEnsemble model returned a 91% sensitivity for high_risk which means almost all high_risk credit was determined. Even though the sensitivity was favorable, the low precision for high_risk was still very low. Therefore, the outcome of this model still detects some low risk credit to be falsely determined as high_risk. This would result in the bank losing revenue by missing out on good candidates for loans. For the purpose of credit risk determining, a low precision rate is not tolerable as it will lead to missed lending opportunities. I would not recommend any of the models to predict credit risk for these reasons. Some other models would have to be tested or perhaps other features for determining credit risk would have to be accounted for in future models.


