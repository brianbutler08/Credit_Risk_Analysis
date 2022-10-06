# Credit Risk Analysis

# Overview of the Analysis

For this project, we utilized six different supervised machine learning models to predict credit risk. Three of them used resampling techniques (oversampling *or* undersampling), one used a combination of over- and undersampling and two were ensemble classifiers. 

**Resampling Models**
- Used the RandomOverSampler and SMOTE algorithms to oversample the data
- Undersampled the data using the ClusterCentroids algorithm
- Used a combination of over- and undersampling with the SMOTEENN algorithm

We used each algorithm to resample the dataset, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report. The use of SMOTEENN was to determine if the results from the combined approach are better at predicting credit risk than just the oversampling and undersampling algorithms.

**Emsemble Classifiers**

We trained and compared two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk, and evaluated each model based on performance.

# Results

For each algorithm or model, we evaluated performance by looking at the accuracy score, generating a confusion matrix and printing a classification report.

## Random Over Sampler

**Accuracy Score**

![AS1](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS1.png)

**Confusion Matrix**

![CM1](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM1.png)

**Classification Report**

![CR1](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR1.png)

- The balanced accuracy is 0.65
- The high risk precision score is 0.01 with a sensitivity of 0.61
- The low risk precision score is 1.0 with a sensitivity of 0.68
- The extreme precision values can be attributed to the very unbalanced nature of the dataset

## SMOTE

**Accuracy Score**

![AS2](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS2.png)

**Confusion Matrix**

![CM2](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM2.png)

**Classification Report**

![CR2](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR2.png)

- The balanced accuracy is 0.62
- The high risk precision score is 0.01 with a sensitivity of 0.61
- The low risk precision score is 1.0 with a sensitivity of 0.64

## Cluster Centroids

**Accuracy Score**

![AS3](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS3.png)

**Confusion Matrix**

![CM3](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM3.png)

**Classification Report**

![CR3](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR3.png)

- The balanced accuracy is 0.62
- The high risk precision score is 0.01 with a sensitivity of 0.61
- The low risk precision score is 1.0 with a sensitivity of 0.43

## SMOTEENN

**Accuracy Score**

![AS4](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS4.png)

**Confusion Matrix**

![CM4](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM4.png)

**Classification Report**

![CR4](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR4.png)

- The balanced accuracy is 0.52
- The high risk precision score is 0.01 with a sensitivity of 0.70
- The low risk precision score is 1.0 with a sensitivity of 0.58

## Balanced Random Forest Classifier

**Accuracy Score**

![AS5](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS5.png)

**Confusion Matrix**

![CM5](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM5.png)

**Classification Report**

![CR5](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR5.png)

- The balanced accuracy is 0.79
- The high risk precision score is 0.03 with a sensitivity of 0.68
- The low risk precision score is 1.0 with a sensitivity of 0.90

## Easy Emsemble Classifier

**Accuracy Score**

![AS6](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/AS6.png)

**Confusion Matrix**

![CM6](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CM6.png)

**Classification Report**

![CR6](https://github.com/brianbutler08/Credit_Risk_Analysis/blob/main/Module_18_images/CR6.png)

- The balanced accuracy is 0.93
- The high risk precision score is 0.06 with a sensitivity of 0.92
- The low risk precision score is 1.0 with a sensitivity of 0.94

# Summary

The primary challenge in developing the best model to assess credit risk is the tremendously unbalanced dataset that we are working with. The relatively low number of high risk loan applications makes it difficult to accurately predict for them. The extremely low (0.01 to 0.06) precision scores don't give us a tremendous amount of confidence in how reliable our positive classifications are. In looking at the balanced accuracy scores, none of the algorithms that utilized resampling techniques resulted in scores that are high enough to have much confidence in. However, the two ensemble models showed a lot more promise in this metric with a score or 0.79 for the balanced random forest classifier and 0.93 for the easy ensemble classifier. Each also displayed high sensitivity scores for both the low and high risk loans.

Because of the precision scores for every model that we tested, it is difficult to recommend any of them for further application. However, if it was necessary to identify the most appropriate one then the easy ensemble classifier would be the best candidate.


