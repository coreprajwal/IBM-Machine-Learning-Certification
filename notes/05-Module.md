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
