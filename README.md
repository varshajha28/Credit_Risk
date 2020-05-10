# Credit_Risk

## Project Overview
The project aims to predict the eligibility of loan applicants for credit using several machine learning algorithms. The algorithms are assessed based on their accuracy score,confusion matrix and classification models  to select the best algorithm to build a best predictive model.
## Resources
- Data Source: LoanData.csv
- Software: Mlenv , Jupyter notebook, Python, Numpy ,Scikit-Learn and Imblearn
 ## Alogirthim used for the project :
 The various algorithim used to predict the model are as follows :
 a) Logistic Regression b) Decision Tree c) Random Forest d) Support Vector Machine e) Naive Bayes f)Bagging and Boosting.
 ## Challenge Overview
The objective of the challenge is to build and evaluate machine learning models to resample the unbalanced classifaction problem of credit risk loan data. The performance of these models will lets us know if they are capable of predicting the credit risk of the loan application. In order to achieve the objective following steps were performed :
**1. Load and Clean up the data : **

The data from the csv file was loaded into a panda dataframe and the basic clean up , binary encoding of the categorical data and the splitting of the data into the training and test set was done .

**2. Naive Ramdom Oversampling:**
The model is built and trained using the RamdonOverSampler method . The balanced accuracy score is 0.65. The Confusion Matrix shows the precison of 0.010 and recall of 0.006 . The Classification report shows the precison of 0.01, recall of 0.69 and F1 score of 0.02 for high risk application . The low risk application shows the precison of 1.00, recall of 0.61 and F1 score of 0.76

**3. SMOTE Oversampling:**
The model is built and trained using the SMOTE method . The balanced accuracy score is 0.66. The Confusion Matrix shows the precison of 0.011  and recall of 0.005 . The Classification report shows the precison of 0.01, recall of 0.63 and F1 score of 0.02 for high risk application . The low risk application shows the precison of 1.00, recall of 0.69 and F1 score of 0.82

**4. Undersampling:**
The model is built and trained using the ClusterCentroids method . The balanced accuracy score is 0.66. The Confusion Matrix shows the precison of 0.006 and recall of 0.009. The Classification report shows the precison of 0.01, recall of 0.66 and F1 score of 0.01 for high risk application . The low risk application shows the precison of 1.00, recall of 0.40 and F1 score of 0.57

**5. Combination (Over and Under ) SMOTENN sampling:**
The model is built and trained using the SMOTEENN method . The balanced accuracy score is 0.53. The Confusion Matrix shows the precison of 0.009 and recall of 0.007 . The Classification report shows the precison of 0.01, recall of 0.72 and F1 score of 0.02 for high risk application . The low risk application shows the precison of 1.00, recall of 0.57 and F1 score of 0.72

## Challenge Summary
Based on the above mentioned data none of the model is adeqaute enough to predict the credit risk for the loan.

## Challenge Extension Analysis and Summary
After performing the similar steps of loading and cleaning the data , the following ensemble techniques were used to see the perfomance of the models :

**Balanced Ramdom Forest:**
The model is built and trained using the Balanced Random Forest method . The balanced accuracy score is 0.76. The Classification report shows the precison of 0.04, recall of 0.67 and F1 score of 0.07 for high risk application . The low risk application shows the precison of 1.00, recall of 0.90 and F1 score of 0.95

**Easy EnsembleAdaBoost:**
The model is built and trained using the Easy EnsembleAdaBoost method . The balanced accuracy score is 0.93. The Classification report shows the precison of 0.09, recall of 0.92 and F1 score of 0.16 for high risk application . The low risk application shows the precison of 1.00, recall of 0.94 and F1 score of 0.97

**Ensemble Summary:**
The easy EnsembleAdaboost method has the highest accuracy rate and F1 score however the precison rate for the high risk is still low . The recall rate however in both the case (high and low risk) is good . This model is very good in predicting the low risk application but it does not perform very good on the high risk application at least in terms of precision. 

