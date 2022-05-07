# Credit_Risk_Analysis
## Purpose
  Credit risk is an inherently unbalanced clssification problem, as good loans easily outnumber risky loans. So we used different techniques to train and evaluate models with unbalanced classes. We used RandomOverSampler and SMOTE algorithms to oversample the data, ClusterCentroids to do the undersample. We also used the over and undersampling using the SMOTEEN algorithm. Then we used the two machine learning models BalanceRandomForestClassifier and EasyEnsembleClassifier to predict credit risk.
  
## Results

  #### RandomOverSampler
  - Balanced Accuracy Score
    
  ![image](https://user-images.githubusercontent.com/56806834/167266244-5edfceef-b43d-407a-a398-071b178da6c2.png)


  - Precision and Recall Scores
  
  ![image](https://user-images.githubusercontent.com/56806834/167266257-feeb24f2-ad8b-47f8-8d56-d4eec1039aad.png)


### SMOTE
  - Balanced Accuracy Score

![image](https://user-images.githubusercontent.com/56806834/167266410-490826ea-208d-4f29-8776-8cd420051dd4.png)


  - Precision and Recall Scores
  
  ![image](https://user-images.githubusercontent.com/56806834/167266420-045e8885-6f9f-4f52-8fde-a3d61bda86cd.png)


### Undersampling
  - Balanced Accuracy Score
  
  ![image](https://user-images.githubusercontent.com/56806834/167266452-2cb03159-5ff1-4524-bbcc-b40a3aa7f236.png)


  - Precision and Recall Scores

  ![image](https://user-images.githubusercontent.com/56806834/167266460-1dc07b48-0705-4f30-a56b-f187cb61453f.png)
  

### SMOTEENN
  - Balanced Accuracy Score
  
  ![image](https://user-images.githubusercontent.com/56806834/167266482-c0cff7ab-6376-484c-82b1-c0a5925a5dd1.png)

  
  - Precision and Recall Scores
  
  ![image](https://user-images.githubusercontent.com/56806834/167266491-6f4ea1df-dd22-4a9a-a584-8b50a0f03825.png)

  
### BalancedRandomForestClassifier
  - Balanced Accuracy Score

  ![image](https://user-images.githubusercontent.com/56806834/167266528-61cd3a38-d42f-4109-95db-aa05e6b1d804.png)


  - Precision and Recall Scores
  
    ![image](https://user-images.githubusercontent.com/56806834/167266546-6116871b-f5b6-469d-9eed-5db278d0d5f6.png)


### EasyEnsembleClassifier
  - Balanced Accuracy Score
  
  ![image](https://user-images.githubusercontent.com/56806834/167266575-60aa6fa5-1c4a-4df4-aefa-2a3eab0b9ad6.png)


  - Precision and Recall Scores

  ![image](https://user-images.githubusercontent.com/56806834/167266582-ac8d6596-5dae-4400-874c-74e2a28bbfa7.png)

  
## Summary

#### Precision
  
  - Looking at all the models' precision scores they all look very similar, which is high precision for low risk. That means if we base our analysis against Precision score, all the models work the sameway. So I cannot recommend one particular model in this case.
  - Having high precision means having a high measure of relevant results returned with limited irrelavant results

#### Recall
  - A high recall indicates the model is able to successfully identify relevant results without mislabeling them as irrrelevant
  - Recall varies for different models. Looking at Recall score it looks like EasyEnsembleClassifier is the best model for credit risk analysis.

#### Accuracy
  - Accuracy is ametric that generally describes how the model performs across all classes. It is useful when all classes are of equal importance.
  - Looking at the Accuaracy score for different models here, it looks like EasyEnsembleClassifier is the best model to do the credit risk analysis here.

From the above observations, I recommend EasyEnsembleClassifier Model to do the credit risk analysis.

  
