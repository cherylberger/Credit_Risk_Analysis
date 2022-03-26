# Credit_Risk_Analysis
#### Cheryl Berger
# Module 17 Challenge Data Analytics

## Overview:
Develop 6 different machine learning models to perform a loan prediction risk analysis for the credit card dataset from LendingClub.  The analysis will be shared with Jill to help resolve an inherent unbalanced classification problem, good loans easily outnumber risky loans. Using imbalanced learn and scikit learn libraries to build and evaluate models using various resampling methods.  Include a summary for Jill explaining which model, if any is preferred when used to predict credit risk. 

## Resources: 

## Results: 

Credit Risk Resampling Techniques, Read the CSV and Perform Basic Data Cleaning
Split the data into train and test sets
![image](https://user-images.githubusercontent.com/94234511/160216200-5d0fc40d-13bd-4c89-92ff-2ba41dbe6941.png)


### Deliverable 1: Use Resampling Models to Predict Credit Risk 

#### Random Oversampling Algorithm
![image](https://user-images.githubusercontent.com/94234511/160216021-efe16d32-8d46-477d-a96a-51792ebe859a.png)
-The balanced accuracy score was 
-The precision for the high credit risk prediction was % while % for the low credit risk predictions 
-The recall (sensitivity) score was

#### SMOTE Oversampling ALgorithm
![image](https://user-images.githubusercontent.com/94234511/160216057-aff0db8f-1386-42c1-b241-7bb23206d159.png)
-The balanced accuracy score was 
-The precision for the high credit risk prediction was % while % for the low credit risk predictions 
-The recall (sensitivity) score was

#### Undersampling using the ClusterCentroids Algorithm
![image](https://user-images.githubusercontent.com/94234511/160216099-06fab599-9b64-4003-a182-fa46f02a13b2.png)
The balanced accuracy score was 
The precision for the high credit risk prediction was % while % for the low credit risk predictions 
The recall (sensitivity) score was


### Deliverable 2: Use the SMOTEENN alogrithm to Predict Credit Risk

#### Combination Oversampling and Undersampling SMOTEENN
![image](https://user-images.githubusercontent.com/94234511/160216149-e5269f80-3355-4336-913a-ab283e6b0a06.png)
The balanced accuracy score was 
The precision for the high credit risk prediction was % while % for the low credit risk predictions 
The recall (sensitivity) score was


### Deliverable 3 Use Ensemble Classifiers to Predict Credit Risk

#### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/94234511/160216351-a9a8fde6-2b74-4029-8dc4-ebef800fb4b6.png)
The balanced accuracy score was 
The precision for the high credit risk prediction was % while % for the low credit risk predictions 
The recall (sensitivity) score was

Next, print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
![image](https://user-images.githubusercontent.com/94234511/160216377-f64e35ad-dbe4-44c8-8910-c481499006f0.png)


#### Easy Ensemble Classifier
![image](https://user-images.githubusercontent.com/94234511/160216453-0715a814-1872-4c0a-82c5-ce01aa675b81.png)
The balanced accuracy score was 
The precision for the high credit risk prediction was % while % for the low credit risk predictions 
The recall (sensitivity) score was

## Summary:

There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)

