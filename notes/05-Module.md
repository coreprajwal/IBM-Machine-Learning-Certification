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

## Explain evaluation of unsupervised learning models
- Evaluation of unsupervised learning models is slightly different than supervised learning model as this doesn't have ground truth or label to cross verify
- we also have to check for the stability of the model and ensure it gives more generalised output and specific to some data on which its trained on
- instead we do evaluation based on various heuristics such as :-
  internal evaluation metrics
  external evaluation metrics
  Generalisability or stability
  Dimensionality reduction
  cluster assisted learning 
  domain experties

## Differentiate their heuristic types and there evaluation of cluster quality

- 1)Internal evaluation metrics :-
  (assess the quality of clustering  and focused on input data)
  silhoutte clustering :
   Silhouette = each person asking “Do I belong here or somewhere else?”
  Davies-bouldin :
  neighborhoods compared to see if they’re distinct.
  Inertia :
  how far residents are from the town center.

- 2)External evaluation metrics :-
  (Uses labeled data to measure the correctness of the model of prediction)

  Adjusted rand-index :-
  Measures how similar your clustering is to the true labels, correcting for chance. ( -1 (bad) , 1 (good) )

  Normalized Mutual Information :-
  Think of two books in different languages telling the same story. NMI checks how much knowing one book (your clustering) tells you about the other (ground truth).

  Fowelks-Mallows Index :-
  Imagine checking pairs of students:-
  “Are they in the same group in my clustering, and also in the true labels?” FMI is high if your clustering is precise and recalls most true pairs.

- 3)Dimensionality Reduction :-
  PCA (Explained Variance Ratio,Reconstruction error (how original data can be reconstructed ))
  t-SNE
  UMAP

## Define Model Validation
- Model validation is a splitting of training data into folds and each models prediction is tested on each fold to get accuracy, this reduces the chances of overfitting model on single dataset.

## Explain data snooping and how to avoid it
Data snooping is when you change or modify data or model after peeking the accuracy for one particular test data set and keep modifying until it gives good accuracy for that particular test data resulting overfitting and less generalisability

## Discuss key strategies for model validation
strategies are cross validation, k -folds of data set and 
stratified cross validation


## Define regularization for linear regression
- Regularization is a technique to reduce overfitting, and prevent model to learn the noise of data



## Compare linear , ridge and lasso regression methods
- ridge regression add a lamda and penalty value to the mean squared error which penalizes the error by squaring the coefficients of each variable, this allows to not let one feature dominate on others and have equal importance

- lasso regression helps to do feature engineerin as it adds mod of each coefficient of variable with lambda to the mse and thus small correlation values get zero and thus not included , therefore the feature engineering

## Define Data Leakage
- Data leakage is when you information from test leaks into your model
- it can happen if features created are based on whole dataset and not only training set
- also happens we provide future data such as accuracy to model and retrain model and test on same test data.
- you weren't carefull while performing train test split, cross validation, and test set

## How to mitigate data leakage
- be carefull with data engineering, don't create feature that leaks future test data info into iteself
- do proper separation while of train test split, cross validation, and test set validation

## Feature importance interpretation and other modeling pitfalls
- In feature importance we only non reduntant features
- Ensure training features are available for real-world deployment
- if two features doesn't directly help in performance in a model ,suppose linear regression then we might remove those features but the same two features would become important in case of other models such as random forest as random forest can identify the interaction between those two features which could explain the target label, hence be carefull with that


- Modelling pitfalls
- Selecting inappropriate features
- Interpretating wrong evaluation metrics
- ignoring class imbalance
- Blind reliance on automation
- Performing "what-if" scenario based on non-causal data