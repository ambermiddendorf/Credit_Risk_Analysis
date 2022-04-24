# Credit_Risk_Analysis
Module 17 - Machine Learning


## Overview of the analysis: 
In this analysis, a credit card credit dataset from LendingClub will be run through a variet of algorithms to find the best machine learning model to predict credit risk. I'll evaluate the performance of each of these models and make a recommendation as to which one to use to predict credit risk.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Oversample
* RandomOverSampler 
** Balanced accuracy score of .6182
** High-Risk recall of .55

* SMOTE
** Balanced accuracy score of .6547
** High-Risk recall of .57

### Undersample 
* ClusterCentroids
** Balanced accuracy score of .6547
** High-Risk recall of .55

### Combonation Oversample and Undersample 
* SMOTEENN 
** Balanced accuracy score of .5442
** High-Risk recall of .72

### Ensemble Classifiers 
* BalancedRandomForestClassifier 
** Balanced accuracy score of .7778
** High-Risk recall of .68
** Top Features

* EasyEnsembleClassifier
** Balanced accuracy score of .9321
** High-Risk recall of .92

## Summary: 
The Easy Ensemble Classifier algorithm did the best job in predicting high-risk credit. The algorithm had an accuracy score of 93.21% and found 92% of high-risk credit, which was a marked improvement over any of the other algorithms I tested. 




