# Credit_Risk_Analysis
#### Cheryl Berger
# Module 17 Challenge Data Analytics

## Overview:
Develop 6 different machine learning models to perform a loan prediction risk analysis for the credit card dataset from LendingClub.  The analysis will be shared with Jill to help resolve an inherent unbalanced classification problem, good loans easily outnumber risky loans. Using imbalanced learn and scikit learn libraries to build and evaluate models using various resampling methods.  Include a summary for Jill explaining which model, if any is preferred when used to predict credit risk. 

## Resources: 

## Results: 

Create the code in Python to perform the analysis, credit_risk_resampling.ipynb.  Load the dependencies for the resampling techniques, using Pandas read the datafile (LoanStats.csv) and perform basic data cleaning. The dataframe can be seen in the jupyter notebook file. Next, make the data easier to manage by gnerating a training data set. Split the data into train and test sets as illustrated below and complete the code to evaluate each machine learning algorithm. 

![image](https://user-images.githubusercontent.com/94234511/160216200-5d0fc40d-13bd-4c89-92ff-2ba41dbe6941.png)

### Deliverable 1: Use Resampling Models to Predict Credit Risk 

#### Random Oversampling Algorithm
![image](https://user-images.githubusercontent.com/94234511/160216021-efe16d32-8d46-477d-a96a-51792ebe859a.png)
 * The balanced accuracy score was 62.5%
 * The precision for the high credit risk prediction was very low, only 1% and 100% for the low credit risk predictions 
 * The recall (sensitivity) score was 60% for high risk and 65% for the low risk predictions.  

#### SMOTE Oversampling ALgorithm
![image](https://user-images.githubusercontent.com/94234511/160216057-aff0db8f-1386-42c1-b241-7bb23206d159.png)
  * The balanced accuracy score was slightly better at 65.1% 
  * However, the low precision for the high credit risk prediction, 1% and 100% for the low credit risk predictions 
  * The recall (sensitivity) score was about the same at 64% and 55% for the high and low credit risk predictions respectively.

#### Undersampling using the ClusterCentroids Algorithm
![image](https://user-images.githubusercontent.com/94234511/160216099-06fab599-9b64-4003-a182-fa46f02a13b2.png)
  * The balanced accuracy score was lower than the oversampling methods at 59.9%
  * The precision for the high credit risk prediction was not improved, again 1% and 100% for the low credit risk predictions 
  * The recall (sensitivity) score was similar for the risk risk predictions at 61% but only 45% for the low risk predictions


### Deliverable 2: Use the SMOTEENN alogrithm to Predict Credit Risk

#### Combination Oversampling and Undersampling SMOTEENN
![image](https://user-images.githubusercontent.com/94234511/160216149-e5269f80-3355-4336-913a-ab283e6b0a06.png)
  * The balanced accuracy score was 63.8%
  * Again, the low precision for the high credit risk predictions was not improved, again 1% and 100% for the low credit risk predictions 
  * The recall (sensitivity) score was lower than the other models at 70% and 57% for the the high and low risk predictions respectively. 

### Deliverable 3 Use Ensemble Classifiers to Predict Credit Risk

#### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/94234511/160216351-a9a8fde6-2b74-4029-8dc4-ebef800fb4b6.png)
 * The balanced accuracy score was 78.8%, improved over the over and under-sampling methods. 
 * The precision for the high credit risk prediction was slighlty better at 4% while still indicative of a high number of false postivies.  The precision was again 100% for the low credit risk predictions 
 * The recall (sensitivity) scores were 76% for the high risk and 91% for the low risk predictions suggesting some improvement in ability to model but still prone to false positives.  
![image](https://user-images.githubusercontent.com/94234511/160218234-85ad49da-aeb3-4b39-bdb2-59c33df6af00.png)

Next, print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
![image](https://user-images.githubusercontent.com/94234511/160216377-f64e35ad-dbe4-44c8-8910-c481499006f0.png)

#### Easy Ensemble Classifier
![image](https://user-images.githubusercontent.com/94234511/160216453-0715a814-1872-4c0a-82c5-ce01aa675b81.png)
 * The balanced accuracy score was 92.5%, considerably improved over the earlier models
 * The precision for the high credit risk prediction was 7% while 100% for the low credit risk predictions 
 * The recall (sensitivity) score was 91% for the high risk predictions and 94% for the low risk.  
![image](https://user-images.githubusercontent.com/94234511/160218256-3f80d4df-712f-45b4-b309-cee297333f22.png)

## Summary:

All of the models will have poor precision for the high credit risk data, resampling may not be the best overall approach for predicting credit risk as there is bias in the data.  The use of the bias reducing algorithms appears somewhat more meaningful in the models and had high accuracy scores.  However, the precision of the high credit risk predictions was still poor at 7%.  The imbalance between presion and senstiivity for the model yields an F1 score=0.14 for the high risk predictions.  This model is prone to false predictions of high credit risk.  Therefore, the bank may be rejecting loan applications that were acutally credit worthy.     

