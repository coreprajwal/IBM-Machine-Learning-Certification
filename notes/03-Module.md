# 📘 Module 3: Building Supervised Learning Model

> 🧠 Summary:  


## 🧩 what is classification?
- classification is process of classifying the category of a variable based on its independent variables

## 🧠 List classification algorithms
- Logistic regression
- KNN
- Decision tree
- Naive Bayes
- Support Vector Machines
- Neural Networks


## 🧠 Multi-class prediction
- multiclass prediction is classifying multiple categories based set of independent varibles
- there are two methods for multi-class prediction:
- one vs all:-
- here we let the 1 algorithm to do the job of classifying, it looks each category one by one and then classifies it
- one ve one:-
- here we use multiple binary classification , each binary classification for each unique category, and voting is done to classify


## 💡 Applications of classification
- churn prediction
- drug prescription based on multi class
- loan default prediction
- Customer segmentation


## What is decision tree
- Decision tree is an machine learning algorithm that helps predict category of a target varible

## How to build decision tree
- Decision tree builds chooses features to split based on information gain
- entropy shows how impurity is there in a particular node
- information gain is opposite of entropy
- information gain also helps to know how imoortant is a certain independent variable
## How decision tree learn
- first a feature is selected based on information gain and set as root node
- the root node gets split into categories of that particular node
- gini index or entropy is calculated to see impurity
- if a node is found pure, meaning- all 0 or all 1
- then it branches to the final value and that itself becomes leaf node, no further division happens
- but if no pure division is there ,then next feature is chose to further divide and we iterate until we get pure split

## Regression tree
- Regression tree is same as decision tree but for continueos target value rather than categories


## Difference between Classification and regression trees
- predicts continuos value rather than class
- split in classificaion happens based on entropy, gini ,information gain but in regression it happens based on mse


## How to regression tree work
- first we choose each of the dataset
- we calculate mse for each node based on some threshold
- then we calculate weighted mse and iterate same for every feature
- the least weighted mse feature with threshold is selected for the split and the data is splited
- variance is checked after each split and for further splitting same process of selecting feature and then calculating mse and weighted mse is done untill we get split of low variance for higher accuracy