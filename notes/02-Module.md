# 📘 Module 2: Linear and Logistic Regression

> 🧠 Summary:  


## 🧩 what is regression?
- linear regression is supervised learning model
- it models a relationship between continuos independent and dependent feature
  
## Types of regression
- Single regression  
- Multiple regression 

## 🧠 Compare Single and Multiple Regression
single regression has one independent feature
Multiple regression has many independent features

## 🧠 Machine Learning Techniques:-


## 💡Applications of Regression
sales prediction
Price estimation
Predictive maintainance
Employment income
Rainfall estimation
Spread of infectious diesease


## Regression Algorithms :-
1.Linear and polynomial regression
2.Random Forest
3.Extreme Gradient Boosting (XG Boost)
4.K-Nearest Neighbour (KNN) Algorithm
5.Support Vector Machines
6.Neural Network

## What is actually a Simple Linear Regression ?\
- Single independent feature corresponds to single dependent feature
- eg:- engine size and co2 emmision

## How single Linear Regression Work?
- you take independent variable , calculate the co2 emmision by using linear regression formula, which is y=0o + 01x (predicted value)
- we calculate difference between actual and predicted for a single point that is the error, then on performing summation of every error on every point and taking its average we get mean error of the whole single linear regression
- we find the best fit line which has least MSE and its called ols regression
  
## why it fails?
- Outliers reduces its accuracy way too much
- Linear model is too simple to capture complexities

## What is multiple linear regression?
- It is extension of simple linear regression
- It uses two or more independent features to estimate a dependent variable
- 

## compare multiple linear regression and simple regression
  - Multiple linear regression is more better model than the simple regression
  - too many feature may make model overfit
  - categorical columns should be converted to numerical columns as they linear regression doesn't understand categories but numerical features
  
## Applications of multiple regression
- Used in education to predict outcomes and explain relationships
- predict impact in "what-if?" scenarios


## pitfalls of multiple linear regression
- Collinear features are no longer independent features

## solutions to pitfalls
- remove redundant variables
- select variables that are most understood,controllable and corelated with target

## regression line:-
- y predicted line in simple linear regression is a line
- in 2 independent variable it becomes plane
- more than 2 , it turns into hyperplane

## Minimize the mse by finding best parameters:-
- mean squared error= summation of (actual - predicted)^2/n
- least squared error= summation of (actual- predicted)^2

- we can get best parameters by reducing the lse 
- we can get best parameters also by using optimization methods such as gradient descent

## Polynomial Regression
- linear ,cubic , quadratic
- Use those which fits the actual point of target variable
- can be directly used by using same linear regression formula, just change the variable into x,x^2,x^3 etc

## Nonlinear Regression
- examples:- random forest, decision tree , knn, neural network etc
-  non linear regression are the relationships between independent variables which cannot be captured with a simple linear regression line
-  includes funcitons like, logrithm,exponential etc

## Applications of non-linear regression
- Compounding investments
- Productivity graph

## Logistic Regression 
- Logistic regression is used to classify target variable if its in binary
- it is also a probability calculator, where if the probability goes beyond the threshold boundary the churn becomes 1 else its 0
## Explain how logistic regression is used
- here we use sigmoid function to squash the result into binary from the probability
- sigmoid function formulat= 1/ 1+e^-x
- Logistic regression is good choice for understanding impact of a certain feature on the target variable,binary classification and finding probability
- we use log loss as evaluation metric

## Applications
- to predict if an employee will stay or not based on income and age
- if a person will get heart attack or not based on bmi , age etc
- classifying things binary

## how to train a logistic regression model
- first take the parameters randomly
- then find the probability of the class it falls
- then calculate the loss function by actual class probability and predicted class probability
- change the parameters slowly until you get the minimum the cost function and have the best parameters
- method used to reduce the cost function is gradient descent, which comes to global minima  

## features of gradient descent and stochastic gradient descent
- gradient descent help find best parameters by adjusting parameters based on reducing the loss function
- it does this by comming to a global minima , also has learning rate, which is basically a step size, if step size is large it might completely miss global minima and if its too small then it might take too long to reach global minima

- Stochastic gradient descent is faster than gradient descent 
- also comes to global minima

##

