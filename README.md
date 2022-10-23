# Credit_Risk_Analysis

## Purpose and Overview of Project
Use statistical reasoning and machine learning in order to evaluate credit card risk. The data will come from a credit card dataset from the lending services company, LendingClub. After evaluating this data sample, two different machine learning models will be compared to reduce any bias that may occur when predicting credit risk.

1. Explain how a machine learning algorithm is used in data analytics.
2. Create training and test groups from a given data set.
3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
5. Compare the advantages and disadvantages of each supervised learning algorithm.
6. Determine which supervised learning algorithm is best used for a given data set or scenario.
7. Use ensemble and resampling techniques to improve model performance.

## Results
# Deliverable 1: Use Resampling Models to Predict Credit Risk
Three machine learning models, RandomOverSamples, SMOTE algorithms, and ClusterCentroids, have been used to evaluate which is better at predicting credit risk. The criteria used for this determination includes balanced accuracy scores, logistic regression classifiers, and classification reports.

-Random Oversampling
![image](https://user-images.githubusercontent.com/108380062/197397923-838530c1-4488-4221-a611-d704604caf28.png)
The balanced accuracy score is 0.6515938052705158.
![image](https://user-images.githubusercontent.com/108380062/197397755-0bfb07c4-70b2-448b-889a-860cdc0edd00.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.62 high risk loans and 0.68 for low risk loans.

-SMOTE Oversampling
![image](https://user-images.githubusercontent.com/108380062/197398389-25709498-6bd8-4014-9184-f6b859a7cc06.png)
The balanced accuracy score is 0.6241876870888075
![image](https://user-images.githubusercontent.com/108380062/197398487-7ce3d65f-aca0-4f25-aea0-1bea93ea1361.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.59 for high-risk loans and 0.66 for low-risk loans.

-Undersampling/Cluster Centroids
![image](https://user-images.githubusercontent.com/108380062/197398696-d898609a-e9e7-4e0a-bf3b-9ce4ee4109ca.png)
The balanced accuracy score is 0.6241876870888075 as it is above in SMOTE.
![image](https://user-images.githubusercontent.com/108380062/197398786-0fa9441f-d815-4b02-adbd-deb7eed77a52.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.60 for high-risk loans and 0.43 for low-risk loans.

#Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
SMOTEENN algorithms will be used with an over and undersampling approach to determine if the results from the combination of approaches are better at predicting credit risk over the resampling algorithms attempted in the first deliverable.

-SMOTEENN algorithm to predict credit risk
![image](https://user-images.githubusercontent.com/108380062/197399037-38e469f5-50e8-4e22-8619-77b15e86867f.png)
The balanced accuracy score is 0.5160196365189295
![image](https://user-images.githubusercontent.com/108380062/197399127-1d078e29-65ab-4656-81eb-431f766686fe.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.70 for high-risk loans and 0.58 for low-risk loans.

#Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Two different ensemble classifiers: Balanced Random Forest Classifier & Easy Ensemble AdaBoost Classifier are used to predict credit risk.

-Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/108380062/197399378-d4b5003d-e847-451d-a16c-2374400a0661.png)
The balanced accuracy score is 0.7877672625306695
![image](https://user-images.githubusercontent.com/108380062/197399437-c3e20fa2-0eb0-4c0d-8e40-4177a5ba7fca.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.67 for high-risk loans and 0.91 for low-risk loans.

-Easy Ensemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/108380062/197399527-60e6b961-1cde-4619-ab5b-434b0d85a092.png)
The balanced accuracy score is 0.925427358175101
![image](https://user-images.githubusercontent.com/108380062/197399611-1047d38e-281f-4cfd-abd3-8494d96893d5.png)
For the precision score, the precision is low for high-risk loans and is high for low-risk loans.
The recall score is 0.91 for high-risk loans and 0.94 for low-risk loans.

##Summary
Balanced accuracy uses sensitivity and specificity to evaluate the performance of a classifier. The balanced accuracy is placed on a scale of 0 to 1. The closer to 1 the balanced accurracy is, the better the prediction of the model. For the credit card risk data set: all of the classifiers tested showed similar recall scores, and all had precision scores as low for high-risk loans and high for low-risk loans. The difference in these learning models occurs in the balanced accuracy score. The Easy Ensemble AdaBoost Classifier outperformed all off the other models significantly with a score of 0.925427358175101. Seeing as none of the other machine learning models had balanced accuracy scores above 0.7877672625306695, the Easy Ensemble AdaBoost Classifier is the best choice when analyzing and predicting credit card risk.
