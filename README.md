
# Credit_Risk_Analysis

# Overview

The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk. In order to complete this task, I used  different methods.

- oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

# Resources

Data Source: LoanStats_2019Q1.csv

Software: Python 3.7.9, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

# Results

Deliverable 1: Use Resampling Models to Predict Credit Risk

- RandomOverSampler model 

The balanced accuracy score is 65%.

The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.

Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

![oversampling_cm](https://user-images.githubusercontent.com/96400887/183689353-c5289cb0-e7a2-45db-b245-ad3fd4d6bb41.png)

![oversampling_analysis](https://user-images.githubusercontent.com/96400887/183689436-71c929b1-684f-47ee-9861-8981ce0cd8dd.png)

- SMOTE Model

The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

![smote_cm](https://user-images.githubusercontent.com/96400887/183689482-32e9c9ec-d798-4f33-b79b-dfd43e2026ee.png)

![SMOTE_Analysis](https://user-images.githubusercontent.com/96400887/183689514-8a37fc11-f5d0-4c00-bf07-96914b1da048.png)

- ClusterCentroids Model

![cluster_analysis](https://user-images.githubusercontent.com/96400887/183693506-d39c1744-8490-4217-aafe-0bc3d50a649d.png)


![combination sampling](https://user-images.githubusercontent.com/96400887/183689981-e1dc0256-5682-4e79-aec7-6e1c52558069.png)

![combinational_analysis](https://user-images.githubusercontent.com/96400887/183689998-7a13781a-d9a6-4103-9cbb-1476fda2da2e.png)

















