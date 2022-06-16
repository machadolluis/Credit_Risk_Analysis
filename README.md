# Credit_Risk_Analysis

## Overview

In this project, we use Python with Jupyter Notebooks to test various machine learning models to predict risk. We use oversampling and undersampling methods, a combined approach with SMOTEENN  as well as bias-reducing ensemble methods.

After evaluating each model, we will make a recommendation on which should be used to predict credit risk the best.

## Results

### RandomOverSampler
![](/images/ros_class_report.png)
Balanced accuracy score = 61.2%

The high_risk precision is only 1%, with a sensitivity of 71%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 61%

### SMOTE
![](/images/SMOTE_class_report.png)
Balanced accuracy score = 65.4%

The high_risk precision is only 1%, with a sensitivity of 63%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 68%

### ClusterCentroids
![](/images/cc_class_report.png)
Balanced accuracy score = 54.4%

The high_risk precision is only 1%, with a sensitivity of 69%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 40%

### SMOTEENN
![](/images/SMOTEENN_class_report.png)
Balanced accuracy score = 64.2%

The high_risk precision is only 1%, with a sensitivity of 71%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 57%

### BalancedRandomForestClassifier
![](/images/brfc_class_report.png)
Balanced accuracy score = 77.6%

The high_risk precision is only 3%, with a sensitivity of 67%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 88%

### EasyEnsembleClassifier
![](/images/eec_class_report.png)
Balanced accuracy score = 93.2%

The high_risk precision is 9%, with a sensitivity of 92%

Because of the large number of low_risk variables, its precision is almost 100% with a sensitivity of 94%

## Summary

All the models show low precision to determine if the credit risk is high.
The ensemble models have shown improvement in those predictions, especially with the sensitivity of high credit risk. However, due to the precision score still being low, the model would still incorrectly predict some low risk credits as high risk. 
We would recommend to not use any of the models used above to predict credit risk for the reasons cited.
