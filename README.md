# Credit-Risk-Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we needed to employ different techniques to train and evaluate models with unbalanced classes. Using the imbalanced-learn and scikit-learn libraries building and evaluating models using resmapling methods will help determine the best possible analysis method to reduce the risk of loss on loan returns.

## Purpose
The main purpose of the Credit Risk analysis is the find the best predictor with the least error. We utilized the imbalanced learned and scikit-learn libraries to predict credit risk from out resampling models. By using these libraries we can evaluate which method provides the prediction with the least error and ensure we have the best resampling model. 

## Results
### Resampling Models
* Naive Random Oversampling
  * From the naive random oversampling, we obtained a balanced accuracy score of about 0.6456 or 65%. A 65% accuracy means that our resampling model will accuratley predict the Credit Risk only 65% of the time, which is insufficient for our analysis. With a 65% accuracry score, credit companies would see several losses due to inaccurate predictions. From this score, we can conclude this is not the best method to predict credit risk.
<img width="652" alt="Screen Shot 2022-05-08 at 9 11 56 PM" src="https://user-images.githubusercontent.com/94096530/167339336-71e6732c-2cc8-435d-bfb0-45bac071b9f7.png">

* SMOTE Oversampling
  * With the SMOTE oversampling, we obtain a balanced accuracy score of 0.6234 or 62%. Thus, the resampling model will accuratley predict credit risk only 62% of the time. We can conclude again that this is not the best model to predict credit risk for our analysis. 
<img width="572" alt="Screen Shot 2022-05-08 at 9 11 45 PM" src="https://user-images.githubusercontent.com/94096530/167339323-f5f9db89-f73f-4cdd-929f-dd25080b840a.png">

* Undersampling
  * Our undersamplig model returns a balanced accuracy score of 0.5293 or 53%. This accuracy score is even less than our Naive and SMOTE sampling models. Again, this is not the optimal model for our analysis. 
<img width="554" alt="Screen Shot 2022-05-08 at 9 14 11 PM" src="https://user-images.githubusercontent.com/94096530/167339552-a5fd58ef-5d49-4a22-afb6-0dd2fd0dcfbc.png">

* Over and Under Sampling -- Combination
  * From the combination sampling model, we obtain a balanced accuracy score of 0.6156 or 62%. So, the combination sampling method is also not a good model for our credit risk analysis. 
<img width="566" alt="Screen Shot 2022-05-08 at 9 16 46 PM" src="https://user-images.githubusercontent.com/94096530/167339753-ea193779-0a21-4c70-8caf-2dc8195d767c.png">

## Ensemble Learners

* Balanced Random Forest Classifier 
  * From the Random Forest Classifier, we obtain a balanced accuracy score of 0.7877 or 79%. Although, this is significantly higher than our resampling models, it still does not prove to be accurate enough. Even at 79% accuracy, this model could still cause credit companies to have several losses.  
<img width="547" alt="Screen Shot 2022-05-08 at 9 23 00 PM" src="https://user-images.githubusercontent.com/94096530/167340271-c037fce6-25e0-4682-bf75-ba9cad70ce7a.png">

* Easy Ensemble AdaBoost Classifier
  * The Easy Ensemble AdaBoost Classifier gave us our highest balanced accuracy at 0.9254 or 93%. This is the highest out of all the previous models we have run. Therefore, we can conclude that this model will accurately predict the credit risk approximatley 93% of the time. This would be the most acceptable method for our credit risk analysis.  
<img width="547" alt="Screen Shot 2022-05-08 at 9 24 51 PM" src="https://user-images.githubusercontent.com/94096530/167340447-d6732d4f-a023-48df-8e85-cbea7b587f6c.png">

## Summary 
After using all six of the resampling and esemble methods for our models, we can conclude that the only model that we can use in our analysis is the Easy Ensemble AdaBoost Classifier. This model gave us a 93% balanaced accuracy score and is the best model to use when predicting credit risk. The other five models have low accuracy rates and are deemed more risky to use in our analysis since they will produce inaccurate credit risk predicions, leading to more losses for credit companies. 
