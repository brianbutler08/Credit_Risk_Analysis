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

**Confusion Matrix**

**Classification Report**

## RandomOverSampler

**Accuracy Score**

**Confusion Matrix**

**Classification Report**
# Summary
