# Credit_Risk_Analysis
oversampling credit score data to evaluate credit risk performance via machine learning modules

## Overview

Jill was impressed with our work we provided early on in the module. Now, we are to apply machine learning to the real-world challenge of credit card risk. Jill asks us to utilize the imbalanced-learn and scikit_learn libraries to evaluate the credit risk models. In this particular issue of credit risk analysis, there is a disparity between the high risk and low risk loans. We will use two machine learning models to predict credit risk. The two machine learning models are BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results
  
* Note that "0" represents "high risk" population and "1" represents "low risk" population
  
### RandomOverSampler Model

![](Resources/balanced_accuracy_score.PNG)
![](Resources/imbalanced_classification_report.PNG)

From the random oversampler model, T=the balanced accuracy score is approximately 60.9%. The high risk precison score for this model appears 1% with a F1 score of 2%. Due to the higer number of those in the low risk population, its precision shows almost a 100% result with a sensitivity of 66%.

### SMOTE Model
 
 ![](Resources/smote_balanced_score.PNG)
 ![](Resources/smote_imbalanced.PNG)
 
After running and evaluating the SMOTE Model, we can see the model is similar to the random sampler model.
- The balanced accuracy score shows approximately a score of 63.5% 
- The high risk precision is about 1% with only 62% which then yeilds a f1 score of 2%
- The precision of this model is also approximately 100% with a sensitivity of 65%.

### Cluster Centroids Model

![](Resources/undersampling_balanced_score.PNG)
![](Resources/undersampling_imbalanced.PNG)

- In this model, the balanced accuracy score is down to 50.2%
- However, the high risk precision score is still appearing as 1% with a 58% sensitivity, thus yeilding a F1 of 1%
- Due to this models higher number of false positives, the low risk sensitivity is appearing as 43%.

### SMOTEENN Model

![](Resources/combination_balanced.PNG)
![](Resources/combination_classification.PNG)

- In this SMOTEENN Model, we observe the balanced accuracy score is 64.9%
- The high risk precision score this time shows a 71% sensitivity with 1% and a F1 score of 2%
- Due to this model also having a greater number of false positives, the low risk sensitivity is 59%
