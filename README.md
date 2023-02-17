# Credit_Risk_Analysis
## Analysis/Overview:

This challenge aims to apply machine learning to solve a real-world challenge: credit card risk.  Credit risk is an unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. 

    1.	We are asked to use imbalanced-learn and sci-kit-learn libraries to build and evaluate models using resampling.
    
    2.	Use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, by oversampling the data using the RandomOverSampler and SMOTE        algorithms, then undersample the data using the ClusterCentroids algorithm. 
    
    3.	Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
    
    4.	Finally, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
    
## Results:

We were required to describe the balanced accuracy scores and the precision and recall scores of all six machine learning models based on three different criteria, and the results are:

### Model One - Naïve Random Oversampling:

       •	Balanced Accuracy Score: 0.6406190665839.  The first model accurately predicts that 64% of the minority class is classified as Oversampled.
       
       •	Precision: The total for the high-risk applicant came out to 0.01 and 1.00 for low-risk applications.  Meaning the precision is low for high-risk applicants           and high for low-risk applicants.
       
       •	Recall: high-risk is 0.72 and 0.65 for low-risk.  This means that 72% of applicants are considered high-risk loans, and 65% are considered low-risk loans.
       
       
![Naive Random Oversampling](https://user-images.githubusercontent.com/114379268/219539966-ba0fef50-cb22-4337-a3ed-3e9e0566104c.png)


### Model Two - SMOTE OVERSAMPLING:
		
      •	Balanced Accuracy Score: The second model balance is 0.6602016551047, which is 66%
      
      •	Precision: The precision and totals for this model are the same as the first model.
      
      •	Recall: high-risk is 0.63 and 0.69 for low-risk. 
      
![SMOTE Oversampling](https://user-images.githubusercontent.com/114379268/219540092-d80884b7-d431-4aa2-9140-2efc7065010e.png)


### Model Three - Undersampling:

      •	Balanced Accuracy Score:  0.5442369453, which predicts that the third model is 54% 
        of the minority class is classified as Underrsampled.
      
      •	Precision: The precision totals are identical to the first and second models.
      
      •	Recall: High-risk is 0.69 or 69%, and low-risk is 0.40 or 40%.
      
![Undersampling cluster](https://user-images.githubusercontent.com/114379268/219540284-8346d3d6-4848-4d2c-b763-c59626975864.png)


### Fourth Model - Combination (Over and Under) Sampling:

      •	Balanced Accuracy Score: 0.54473390510233905
      
      •	Precision: The precision for the fourth model is also identified as the first three models.
      
      •	Recall: high-risk is 0.72 or 72%, and low-risk is 0.57 or 57%.


### Fifth Model – Balanced Random Forest Classifier:

      •	Balanced Accuracy score: 0.7885466545953005
      
      •	Precision: The precision for this model's high-risk numbers is slightly higher than the other models. 
        High-risk is 0.3, but low-risk is still the same,which is 1.00, meaning precision is low for high-risk
        loans and high for low-risk loans. 
      
      •	Recall: High-risk is 0.70 or 70%, and low risk is 0.87 or 87%.
      
![Balanced Random Classifier](https://user-images.githubusercontent.com/114379268/219540912-936460e6-2708-49e1-a398-729f4d58df3c.png)


### Sixth Model –  Easy Ensemble AdaBoost Classifier:

    •	Balanced Accuracy Score: 0.9316600714093861
    
    •	Precision: the high-risk totals in this model are the highest out Of all the other models.
      It’s 0.09, but the low risk is still the same, which is 1.00
    
    •	Recall: high-risk is 0.92, and low-risk is 0.94
    
    
![Easy Enselmble Adaboost](https://user-images.githubusercontent.com/114379268/219540971-88e37395-5d51-44dc-af24-86a5f11859d7.png)


    
## Summary:

We evaluated different learning machines to determine which models best predicted credit risk.  We oversampled, undersampled, and did a combination of both.  And most of the models had the same results in the balanced accuracy score and precision and recall.  But the one that was better than the rest of the models was the Easy Ensemble AdaBoost Classifier.  It has a high accuracy score; it scored 93%, close to 100%.  And it also gave great numbers in precision and made it the best machine-learning model for identifying credit card analysis.  Even though the balanced accuracy score was high, the low risk was still 1.00, like the other models. Meaning precision is high for low-risk loan applicants.
