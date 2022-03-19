# Analysis Overview
The purpose of this analysis was to apply machine learning to analyze credit card risk. 
Due to the nature of the data, which is inherently unabalanced, multiple machine learning algorithms were applied. This was done to determine which algorithms, if any, were most accurate and better to use for predicting credit risk. 

# Results
A total of six different models were used. The results of each are noted below. 

## Random Oversampling
 - Balanced accuracy score:  63.67%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  62%
 - High-risk F1 value: 2%
 <br>
 ## SMOTE
 - Balanced accuracy score:  63.03%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  62%
 - High-risk F1 value: 2%
 <br>
## Cluster Centroids Undersampling
 - Balanced accuracy score:  63.03%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  60%
 - High-risk F1 value: 1%
 <br>
## SMOTEENN
 - Balanced accuracy score:  63.76%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  70%
 - High-risk F1 value: 2%
 <br>
## BalancedRandomForestClassifier
 - Balanced accuracy score:  78.78%
 - High-risk precision score:  4%
 - High-risk Sensitivity:  67%
 - High-risk F1 value: 7%
 <br>
## EasyEnsembleClassifier
 - Balanced accuracy score:  92.54%
 - High-risk precision score:  7%
 - High-risk Sensitivity:  91%
 - High-risk F1 value: 14%
 <br>

# Summary
Of all six models, the Easy Ensemble Classifier model had the highest balanced accuracy (92.54%) and sensitivity (91%). 
Due to the nature of the imbalanced data, with only a very small percentage being high-risk, the focus is on the ability of the model to accurately predict the high-risk classification. 
Based on the results, the best option of the six models would be the EasyEnsembleClassifier model based on the fact that it has the highest accuracy, sensitivity, precision and F1 values of all six models. 
However, even though the EasyEnsembleClassifier was the most accurate it still has flaws in correctly predicting high-risk. The lender will want to review further to determine if this is an acceptable level of risk with the model. If not, further adjustments to the model or different options should be explored. 
