# 📘 Module 5:

> 🧠 Summary:  


## 🧩 Define train-test-split :
- train test split is that we split data into train set and test set, where on train set we train the model and evaluate based on test set of how well the model is performing and how accurate is it
  
## Describe Confusion Matrix,accuracy,precision,recall and F1 score metric :

These are Classification Evaluation Techniques :-

- Confusion Matrix:-
  consists on True positives,False positives,True negative, False negative
  TRUE/FALSE (Actual lable) and Positve/Negative (Models label)

- Accuracy :-
  Accuracy is ratio of how well model is giving same lable as actual lable

- Precision :-
  How many of them are True Positives from total number Positives predicted
  ("When I shoot, how accurate am I?")

- Recall :-
  how many of total Actual Positives were catched by models prediction.
  ("Did I hit all the targets?")

- F1-score :-
  If both precision and recall are important we use F1 harmonic mean.

## 🧠 Explain need to evaluate regression models :
- regression model can give also give wrong prediction and to keep in chechk and compare if it actually is giving expected output or not we need to evaluate regression models

## 🧠 Define the error of model
- Error of model is difference between predicted and actual point

## 💡Define regression metrics and evaluation techniques
- regression metrics are mean absoulute error (mae),mean squared error (mse),root mean squared error (rmse),r2 score

Explained variance= summation of y(hat)-y(mean)
Unexplained variance= summation of yi - y(hat)
Total variance= summation of yi - y(mean)
r2 variance= unexplained variance / total variance

## Compare different regression metrics