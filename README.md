# Credit_Risk_Analysis

## Overview of Analysis

This analysis uses maching learning models on a credit card dataset from LendingClub to analyze credit card risk. Diffeent models from imbalanced-learn and scikit-learn libraries are used to build and evalute models using resampling to deterimine high_risk and low_risk classes. First the data is oversampled using RandomOverSampler and SMOTE algorithms, and undersampled using ClusterCentroids algorithm. Then a combinatorial approach SMOTEENN, over and undersampling. Finally, in order to redcue bias BalancedRandomForestClassifier and EasyEnsembleClassifier models are use. Each model will be evaluated on its performance to determine if they should be used to evalute the credit risk.

### Results
> RandomOverSampler

* Balanced accuracy score: 
    0.643
* Precision: 
    High_risk 0.01 
    low_risk 1.00
* Recall scores: 
    High_risk 0.61
    Low_risk 0.68

> SMOTE

* Balanced accuracy score: 
    0.632
* Precision: 
    High_risk 0.01
    Low_risk 1.00
* Recall scores: 
    High_risk 0.61
    Low_risk 1.00

> ClusterCentroids 

* Balanced accuracy score: 
    0.529
* Precision: 
    High_risk 0.01
    Low_risk 1.00
* Recall scores: 
    High_risk 0.61
    Low_risk 0.45

> SMOTEENN

* Balanced accuracy score: 
    0.529
* Precision: 
    High_risk 0.01
    Low_risk 1.00
* Recall scores: 
    High_risk 0.72
    Low_risk 0.55

> BalancedRandomForestClassifier

* Balanced accuracy score: 
    0.666
* Precision: 
    High_risk 0.72
    Low_risk 1.00
* Recall scores 
    High_risk 0.33
    Low_risk 1.00

> EasyEnsembleClassifier

* Balanced accuracy score: 
    0.649
* Precision: 
    High_risk 0.93
    Low_risk 1.00
* Recall scores: 
    High_risk 0.30
    Low-risk 1.00



#### Summary

In summary the RandamoOversampler accuracy of predicting credit risk is  63%, precision high_risk low at 0.01, precission low_risk high high at 1.00, recall high_risk high at 0.61 and high low_risk 0.68. The SMOTE accuracy score of predicting credit risk is also 63%, precision for high_risk low at 0.01 and low_risk high at 1.00, recall scores high_risk high at 0.61 and low_risk high at 1.00. The ClusterCentroids accuracy of predicting credit risk is 53%, precision for high_risk 0.01 and low_risk 1.00, recall high_risk 0.61 and low_risk 0.45. The SMOTEENN model accuracy of predicting credit risk is 52%, precision for high_risk is low at 0.01 and low_risk high at 1.00, recall scores high_risk high at 0.72 and low_risk decent at 0.55. The BalancedRandomForestClassifier accuracy of predicting credit risk is 67%, precision for high_risk is high at 0.72 and low_risk high at 1.00, recall for high_risk low at 0.33 and low_risk high at 1.00. The EasyEnsembleClassifier accuracy of predicting is 64%, precision high_risk high at 0.93 and low_risk high at 1.00, recall for high_risk low  at 0.30 and low_risk high at 1.00. Based on the results would recommend using the SMOTEENN because of its high sensitivity of 72% to identify true high_risk indivuals.


