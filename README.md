# Credit Risk Analysis

## Overview

-	The purpose of this analysis is to evaluate different models in machine learning to assess their performance in predicting credit risks for a peer-to-peer lending services company.


## Results

-	Oversampling:
-	Accuracy: 66%, Precision: High Risk: 1%, Low Risk: %100, Recall: HR: 66%, LR: 67%
![Oversampling](/Images/Oversampling.PNG)

-	SMOTE Oversampling:
-	Accuracy: 63%, Precision: High Risk: 1%, Low Risk: %100, Recall: HR: 62%, LR: 64%
![SMOTE Oversampling](/Images/SMOTE_Oversampling.PNG)

-	Undersampling:
-	Accuracy: 59%, Precision: High Risk: 1%, Low Risk: %100, Recall: HR: 61%, LR: 57%
![Undersampling](/Images/Undersampling.PNG)

-	Combination Sampling:
-	Accuracy: 64%, Precision: High Risk: 1%, Low Risk: %100, Recall: HR: 70%, LR: 57%
![Combination Sampling](/Images/Combination_Sampling.PNG)

-	Balanced Random Forest Classifier:
-	Accuracy: 78%, Precision: High Risk: 4%, Low Risk: %100, Recall: HR: 65%, LR: 90%
![Balanced Random Forest](/Images/Balanced_Random_Forest_Classifier.PNG)

-	Easy Ensemble AdaBoost Classifier
-	Accuracy: 92%, Precision: High Risk: 5%, Low Risk: %100, Recall: HR: 93%, LR: 90%
![Easy Ensemble AdaBoost](/Images/Easy_Ensmeble_AdaBoost_Classifier.PNG)


## Summary

-	After observing the results of the different models, both oversampling, the undersampling, and combination models returned around 60% accuracy scores with only 1% of credit being returned as high risk.  They also had low percentages on recall of credit being accurately evaluated.  The balanced random forest classifier had a 70% accuracy score and returned 4% credit as high risk, but the recall of high risk and low risk credit showed a 25% variance.  Finally, the model I recommend for evaluating credit riskiness is the Easy Ensemble AdaBoost Classifier.  It returned with 92% accuracy, 5% of the credit were high risk, and the recall for high risk and low risk cards were 93% and 90%.
The Easy Ensemble learning model makes predictions based of several different models.  By combining multiple models, it increases the performance and accuracy of the model.  This is important when classifying high risk credit candidates for loans.

## Resources
- Data Source: LoanStats_2019Q1.csv
- Tools: Jupyter notebook, Python (sklearn, imblearn, collections, numpy, pandas)
