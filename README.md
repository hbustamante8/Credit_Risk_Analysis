# Credit_Risk_Analysis

##Overview of the Analysis

The purpose of this project is to build and evaluate several machine learning models to predict credit risk through the use of Python. After evaluating each model, a recommendation on which one is the best fit to predict credit risk.

Resources used:
* Data Source: LoanStats_2019Q1
* Software used: Jupyter Notebook, Python 3.7, Anaconda Navigator 2.1.1


## Results of all Machine Learning Models

### RandomOverSampler model

![image](https://user-images.githubusercontent.com/96553992/167510525-ac6c2fc1-8a2f-429d-8bee-06475dd8bd82.png)

* The accuracy score for the model is 65%.
* The high risk precision is about 1% and only 62% sensitivity which makes a F1 score of 2%.
* The high number of low risk population, its precision almost 100% with a sensitivty score 68%.

SMOTE Model

![image](https://user-images.githubusercontent.com/96553992/167732926-deedc72e-7b2e-4e49-a8cd-d43629913f67.png)

* The results are fairly similar to the previous model.
* The balanced accuracy score is 62%.
* The high_risk precision is about 1% with about 61% sensitivity.
* As a result of the high number of low_risk population, the precision is almost 100% with a sensitivty of 64%.

ClusterCentroids Model

![image](https://user-images.githubusercontent.com/96553992/167737587-c0e43a49-dac2-4743-aa6c-7dc36c9dcb57.png)

* In this model, the accuracy score is lower compared to previous models at 51%.
* The high_risk precision continues to be at about 1% with an F1 score around 1%.
* The high number of false positives lead the low sentiivty risk to be a low 44%.


SMOTEENN Model

![image](https://user-images.githubusercontent.com/96553992/167738819-a8f0e95a-fb7a-4358-b107-1ca7f69657c4.png)

* The acccuracy score for this model is 65%.
* The high_risk precision is still about 1% while the sensitivity is 69%. Thus, results in an F1 score of only 2%.
* The low_risk sensitivity is a low 62%.




