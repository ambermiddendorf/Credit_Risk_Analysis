# Credit_Risk_Analysis
Module 17 - Machine Learning


## Overview of the analysis: 
In this analysis, a credit card credit dataset from LendingClub will be run through a variet of algorithms to find the best machine learning model to predict credit risk. I'll evaluate the performance of each of these models and make a recommendation as to which one to use to predict credit risk.

## Results: 

### Oversample

* RandomOverSampler
  * Balanced accuracy score of .6182
  * High-Risk recall of .55
![ROS_Scores](https://user-images.githubusercontent.com/95837693/164953010-6c307b2d-2034-4061-aab8-ea2f86a103d8.PNG)

* SMOTE
 * Balanced accuracy score of .6547
 * High-Risk recall of .57
![SMOTE_Scores](https://user-images.githubusercontent.com/95837693/164953070-69f56b70-8a60-4d36-a556-ede94f39102a.PNG)

### Undersample 
* ClusterCentroids
  * Balanced accuracy score of .6547 
  * High-Risk recall of .55
![CC_Scores](https://user-images.githubusercontent.com/95837693/164953085-14baa952-75dc-46bf-8cde-dd95f692706f.PNG)

### Combonation Oversample and Undersample 
* SMOTEENN 
  * Balanced accuracy score of .5442
  * High-Risk recall of .72
![SMOTEEN_Scores](https://user-images.githubusercontent.com/95837693/164953097-0791c2a8-d289-49e5-8510-15f81deb0614.PNG)

### Ensemble Classifiers 
* BalancedRandomForestClassifier 
  * Balanced accuracy score of .7778
  * High-Risk recall of .68
  ![BRF_Scores](https://user-images.githubusercontent.com/95837693/164953112-03cf6edc-9900-4213-8f85-2dde89f11a5e.PNG)

  * Top Features
  
![features](https://user-images.githubusercontent.com/95837693/164953121-658f1473-5014-4064-8915-1a9fe5b73f71.PNG)

* EasyEnsembleClassifier
  * Balanced accuracy score of .9321
  * High-Risk recall of .92
![EEC_Scores](https://user-images.githubusercontent.com/95837693/164953131-fa78b3f6-b964-4fc8-9e17-700fdfff8ecf.PNG)

## Summary: 
The Easy Ensemble Classifier algorithm did the best job in predicting high-risk credit. The algorithm had an accuracy score of 93.21% and found 92% of high-risk credit, which was a marked improvement over any of the other algorithms I tested. 




