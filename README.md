# Credit_Risk_Analysis

## Purpose

This project is to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results:
None of the random sampling met the standard for corporate use as their precision is very low. The images below displays the precision for each of the models.

Naive Random Oversampling:


![Naive Random Oversampling](/Naive_Random_Oversampling.PNG)

SMOTE Oversampling:


![SMOTE Oversampling](/SMOTE_Oversampling.PNG)


Undersampling:


![Undersampling](/Undersampling.PNG)

Combination (Over and Under) Sampling:


![Combination (Over and Under) Sampling](/Combination.PNG)

Random forest has high precision, however it has low recall and hence this cannot be used. High precision means that when it marks something as high risk, its very probable that it is actually high risk however since it has a low recall it is not marking all the high risk as high risks. The ADAboost has higher recall but lower precision and therfore it cannot be used. The images below displays the summary for each of the models.

Balanced Random Forest Classifier:


![Balanced Random Forest Classifier](/Balanced_Random_Forest_Classifier.PNG)

Easy Ensemble AdaBoost Classifier:


![Easy Ensemble AdaBoost Classifier](/ADAboost.PNG)

## Summary

In summary none of these models are up to par for commercial standards. 

They all have very low precision or low recall. 
