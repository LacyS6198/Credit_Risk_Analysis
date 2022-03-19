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

![Oversample](https://user-images.githubusercontent.com/93630042/159132286-204795b4-9a17-4206-a65d-deec083de917.png)

## SMOTE
 - Balanced accuracy score:  63.03%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  62%
 - High-risk F1 value: 2%

![smote](https://user-images.githubusercontent.com/93630042/159132300-184c07e0-6433-4f1a-845e-953dd37a5c57.png)


## Cluster Centroids Undersampling
 - Balanced accuracy score:  63.03%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  60%
 - High-risk F1 value: 1%

![cluster](https://user-images.githubusercontent.com/93630042/159132308-8789dee8-aca2-4b2d-b140-76622ba45e70.png)

## SMOTEENN
 - Balanced accuracy score:  63.76%
 - High-risk precision score:  1%
 - High-risk Sensitivity:  70%
 - High-risk F1 value: 2%
<br>
![smotten](https://user-images.githubusercontent.com/93630042/159132192-5c48d965-8556-45ad-ab15-d89b55ff1971.png)
<br>
## BalancedRandomForestClassifier
 - Balanced accuracy score:  78.78%
 - High-risk precision score:  4%
 - High-risk Sensitivity:  67%
 - High-risk F1 value: 7%
<br>
![brfc](https://user-images.githubusercontent.com/93630042/159132199-80edb251-6957-406f-9b69-bee78dc50ce5.png)
<br>
## EasyEnsembleClassifier
 - Balanced accuracy score:  92.54%
 - High-risk precision score:  7%
 - High-risk Sensitivity:  91%
 - High-risk F1 value: 14%
<br>
![eec](https://user-images.githubusercontent.com/93630042/159132207-bfea0e26-46db-4261-a81f-5c50840907cb.png)
<br>

# Summary
Of all six models, the Easy Ensemble Classifier model had the highest balanced accuracy (92.54%) and sensitivity (91%). 
Due to the nature of the imbalanced data, with only a very small percentage being high-risk, the focus is on the ability of the model to accurately predict the high-risk classification. 
Based on the results, the best option of the six models would be the EasyEnsembleClassifier model based on the fact that it has the highest accuracy, sensitivity, precision and F1 values of all six models. 
However, even though the EasyEnsembleClassifier was the most accurate it still has flaws in correctly predicting high-risk. The lender will want to review further to determine if this is an acceptable level of risk with the model. If not, further adjustments to the model or different options should be explored. 
