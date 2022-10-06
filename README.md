# Credit_Risk_Analysis

# Overview of the Analysis

For this project, we developed several supervised machine learning models to predict credit risk.

**Resampling Models**
- Used the RandomOverSampler and SMOTE algorithms from imbalanced-learn to oversample the data
- Undersampled the data using the ClusterCentroids algorithm
- Used a combination of over- and undersampling with the SMOTEENN algorithm

We used each algorith to resample the dataset, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report. The use of SMOTEENN was to determine if the results from the combined approach are better at predicting credit risk than just the oversampling and undersampling algorithms.

**Emsemble Classifiers**

We trained and compared two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk, and evaluated each model based on performance.

# Results

For each algorithm or model, we evaluated performance by looking at the accuracy score, generating a confusion matrix and printing a classification report

## RandomOverSampler

**Accuracy Score**

![AS1]()

**Confusion Matrix**

![CM1]()

**Classification Report**

![CR1]()

## SMOTE

**Accuracy Score**

![AS2]()

**Confusion Matrix**

![CM2]()

**Classification Report**

![CR2]()

## ClusterCentroids

**Accuracy Score**

![AS3]()

**Confusion Matrix**

![CM3]()

**Classification Report**

![CR3]()

## SMOTEENN

**Accuracy Score**

![AS4]()

**Confusion Matrix**

![CM4]()

**Classification Report**

![CR4]()

## Balanced Random Forest Classifier

**Accuracy Score**

![AS5]()

**Confusion Matrix**

![CM5]()

**Classification Report**

![CR5]()

## Easy Emsemble Classifier

**Accuracy Score**

![AS6]()

**Confusion Matrix**

![CM6]()

**Classification Report**

![CR6]()

# Summary
