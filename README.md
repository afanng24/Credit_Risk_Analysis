# Credit Risk Analysis

## Overview of Project
The objective of Credit Risk Analysis is to apply machine learning to solve the real world challenge of credit card risk. To achieve our goal we will use the RandomOverSampler and SMOTE algorithms to oversample the dataset. Afterwards, we will undersample the data using the ClusterCentroids algorithm. In the end we will compare between the BalancedRandomForestClassifier and EasyEnsembleClassifier to see which one reduces bias to predict credit risk.
## Resources
**Source of Data** : LoanStats_2019Q1.csv 

**Software** : Python, Pandas, Jupyter Notebook

## Results

- The RandomOverSampler has a balanced accuracy score of just under 66% with a predicted high risk of 73 and predicted low risk of 28. 

![RandomOversamplingResults](https://user-images.githubusercontent.com/82983000/129909679-191b1836-c275-4cb5-9328-a468d9fe3225.png)

- The SMOTE Oversampling has a balanced accuracy score of 64% with a predicted high risk of 61 and predicted low risk of 40.

 ![SmoateOversamplingResults](https://user-images.githubusercontent.com/82983000/129909890-6562e04c-6082-4162-9283-fc9977a6516b.png)
 
- The ClusterCentroids resampler has a balanced accuracy score of 65% with a predicted high risk of 70 and predicted low risk of 31.

 ![ClusterCentroidsRsults](https://user-images.githubusercontent.com/82983000/129910050-15102f0c-1d1f-4615-a899-e0b69c30fe01.png)

- The SMOTEENN resampler has a balanced accuracy score of 54% with a predicted high risk of 73 and predicted low risk of 28.

 ![SmoteenOverUndersamplingResults](https://user-images.githubusercontent.com/82983000/129910274-138a30ad-f72b-4aaf-b8ec-8d8ff80492d6.png)
 
- The BalancedRandomForestClassifier has a balanced accuracy score of 79% with a predicted high risk of 71 and predicted low risk of 30.

 ![BalancedRandomForestResults](https://user-images.githubusercontent.com/82983000/129910544-30c3b2e7-415c-4331-8699-192cf9dd6fd2.png)
 
- The Easy Ensemble AdaBoost Classifier has a balanced accuracy score of 93% with a predicted high risk of 93 and predicted low risk of 8.

 ![EasyEnsembleResults](https://user-images.githubusercontent.com/82983000/129910674-9bafdc91-1df7-4bbb-8ac9-1614777e16a4.png)
 


## Summary
Across the board the precision matrix is the same for every model, that is very low and not applicable. Most of the models generate a slightly above 50% accuracy rate which is not effective when it comes to analysing high risk loans. The only exception is the EasyEnsembleClassifier with a balanced accuracy score of 93% making it the most accurate model compared to the other machine learning models. Therefore, the EasyEnsembleClassifier should be the only one to be used to reduce bias to predict credit risk. 
