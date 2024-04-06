# Credit-Scoring using Logistic Regression

As a data science intern at ID/X Partners (Virtual Internship Program), I was assigned to make a credit risk analysis from lending company. My objective here is to make a good prediction model that can clasify whether borrowers are good or not.

I used logistic regression as a model to predict credit risk and implemented weight evidence & information values to perfrom feature selection

Metrics used in this project are ROC-AUC score and KS-Statistic

My goals here are:

1.build a prediction model with good ROC-AUC score (>0.8) and good KS-Statistic score (>0.45)
2.build credit score (score card) each borrower and treshold recommendation list

# Feature Engineering and Feature Selection

Before implementing weight of evidence and information value method, we have 27 features consist of 4 categorical features and 23 numeric features. We combined features that have similar weight of evidence and dropped those who didn't follow rule of thumb. After implementing selection method, now we have dataset that consist of 466k records and 85 features

# Modeling

We used logistic regression to predict whether the borrower will be a good borrower or not. We also used AUC score and KS-Statistic as our evaluation metric. After performing hyperparameter tuning and feature selection, the results are :

1.AUC Training Score : 0.847
2.AUC Testing Score : 0.848
3.KS Statistic : 0.552
![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/e1f795cd-ae80-4922-9a59-d4a266f8e4da)

# Feature Importance:

1.Last Payment:5 Month Borrowers who made the last payment in the past 5 months, their odds of being a good loan borrowers will increase by 1.9 times
2.Last Payment:5-7 Month Borrowers who made the last payment in the past 5-7 months, their odds of being a good loan borrowers will increase by 1.7 times 3.Interest Rate: 5.3%-7.4% Borrowers with an interest rate of 5.3%-7.4%, their odds of being a good loan borrowers will increase by 1.5 times

# Credit Score Card:

![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/c8f0fdbb-443d-45be-a4b4-85461c75577b)

![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/cf0e9052-4e79-4e3e-a056-b9237781c2a9)

# Insights:

![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/01786d44-ccc6-4fcc-b249-b1fe44d89494)


![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/55f89974-0bad-4413-9ee3-5f05b70da96f)


![image](https://github.com/Satyashreet-Behura/Credit-Scoring/assets/141150927/7885fb1f-b6e9-4ecf-bcc9-84faa7169e50)





