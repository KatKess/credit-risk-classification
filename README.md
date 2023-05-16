# credit-risk-classification

Analysis Overview: 
The purpose of this analysis is to use machine learning to see how well it can predict if a consumer's healthy (low-risk) or unhealthy (high-risk) credit score if they were to be given a loan. It is to decide how credible a consumer is for being given or not given a loan. The data used is from  historical lending activity from a lending service.  

Results:
From Machine Learning Model 1: 
Balanced Accuracy Score: 0.9520479254722232

From Confusion Matrix: 
Confusion Matrix of Testing Data: 
[[18663   102]
 [   56   563]]
 
From Classification Report: 
precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384 

This first model was better at predicting low-risk loans more so than high-risk loans, with a balanced accuracy score of almost 95%. 

From Machine Learning Model 2: 
Balanced Accuracy Score: 0.9936781215845847

From Confusion Matrix: 
Confusion Matrix of Resampled Data: 
[[18649   116]
 [    4   615]]
 
 From Classification Report: 
  precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

From this second model, the balanced accuracy score was almost 99%. The second model predicts high-risk loans better than the first one. 

Summary: 
Based on the balanced accuracy score and recall, the second model is a best fit for predicting high-risk loans, while the first and second model can predict low-risk loans. The confusion matrix predicts a bit more false negatives in the second model, and it also has a less amount of false positives. Because of this, I would recommend using the logistic regression model over the first model. 
