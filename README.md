
# Credit_Risk_Analysis

# Overview

The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk. In order to complete this task, I used  different methods.

- oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

# Resources

- Data Source: LoanStats_2019Q1.csv

- Software: Python 3.7.9, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

# Results

### Deliverable 1: Use Resampling Models to Predict Credit Risk

- RandomOverSampler Model 

The balanced accuracy score is 65%.

The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.

Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.



![oversampling_analysis](https://user-images.githubusercontent.com/96400887/183689436-71c929b1-684f-47ee-9861-8981ce0cd8dd.png)

- SMOTE Model

The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.



![SMOTE_Analysis](https://user-images.githubusercontent.com/96400887/183689514-8a37fc11-f5d0-4c00-bf07-96914b1da048.png)

- ClusterCentroids Model

Here the balanced accuracy score is down to about 52%.
The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%.


![cluster_analysis](https://user-images.githubusercontent.com/96400887/183693506-d39c1744-8490-4217-aafe-0bc3d50a649d.png)


### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

- SMOTEENN Model 

The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.

![combinational_analysis](https://user-images.githubusercontent.com/96400887/183689998-7a13781a-d9a6-4103-9cbb-1476fda2da2e.png)


### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

- Balanced Random Forest Classifying

The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

<img width="568" alt="random_forest" src="https://user-images.githubusercontent.com/96400887/183697354-5328bb50-1fa3-4bd7-9154-66664bf179fd.png">


- Easy Ensemble Classifying

Now, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.



<img width="565" alt="easy_ensemble" src="https://user-images.githubusercontent.com/96400887/183697380-ffeb4a5f-b9ae-4419-8a75-141c29fd5c75.png">


# Summary

- All the Models analysis is trying to find the best model that can detect if a loan is high risk or not. Becasue of that, we need to find a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk.

- The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.
The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. On another hand, with a low precision. 

- After analyzing all these statastics I would recommend to use Easy Ensemble Classifying model for predicting high risk loans.























