# 📘 Module 1: Introduction to Machine Learning

> 🧠 Summary:  
In this Module we are basically going to learn about overview or summary of the whole course and The Fundamentals of Machine Learning , types of learning approaches , important concepts and real world applications. 

---

## 🧩 What is Machine Learning?
- AI comprises of Machine Learning, Deep Learning, Natural Language Processing, Computer Vision, Generative Ai

-Deep learning is subset of Machine Learning and Machine learning is subset of Generative Ai
-Machine Learning basically is related to algorithms (we give data, it learns patterns, gives prediction)
-Deep Learning is about the Multi- Layered Neural Networks 
-Generative Ai is more advanced

---

## 🧠 Types of Machine Learning
- Supervised:-learns on labeled data
- Unsupervised:- Doesn't follow a particular algorithm but learns from patterns (no labels)
- Semi-Supervised:- trains model with limited labeled data
- reinforcement:- Learns from feedback of the environment

---
## 🧠 Machine Learning Techniques:-
-Classification:- Classifies into categories eg:- dieseas is mallignant or not, exoplanet or not
-Regression:- It has continuos values at every point
-Clustering:- Groups similar data
-Association:- Things or events that co-occur
-Anomaly detection:- to know unsual or abnormal cases.
-Sequence Mining- Predict next event
-Dimensionality reduction:- to reduce data size
-Recommendation system:- associate people's preferences 


## 💡 Real-World Applications

- Spam detection
- Product recommendations
- Medical diagnosis
- Netflix and Amazon recommendation
- Loan aprooval

## Machine learning life-cycle
1.Problem definition
2.Data Collection
3.Data Preparation
4.Model development and evaluation
5.Model Deployment

ETL:- Extract,Transform,Load
-Consists of data collection and data preparation


## Describing importance and requirements of each process in life cycle:-
1.Problem definition:- 
-it should be aligned with clients need

2.Data Collection:- 
-we'll for what data is available in the company and identify sources (user data,inventory or product data,other data like saved products , likes products etc)
-then joining, merging ,aggregating etc is done to make one dataset

3.Data Preparation:-
- when data collected from multiple sources, it can have missing data,errors, different formatting
- clean data to remove irrelevant data
- remove extreme values
- missing values removed or replaced
- each column should be in proper format
- create new feature
- correlation analysis (EDA)
- Identify plan train test split (test set can be random or recent one)(make sure there is atleast one transaction by same person on training set)
  
4.Model development and evaluation :-
- use existing frameworks for model
- identify technique:-
  a. content-based filtering :-it finds similarity between product based on content), its done by calculating similarity score between products purchased by same user and recommend product with high similarity (considering there can be other factors for this decision)
  b. collaborative-based filtering:- It finds similar customers based on product liking,bucket users based on there charactericstics (age,skin type,region)
  - Evaluation:-
 a.test model on never-seen-data
 b.further evaluation by testing the model on small set of people's recommendation system and take feedback

5.Model Deployment:-
- model is ready for production, and needs to be deployed on the the respective app and website
- continue tracking performance even after deployment
- retrain model based on new information

## who are Ai Engineers vs Data Scientist
- Ai engineers are those who harness solutions from generative ai

Ai-Engineers:-
- Ai-System Builders
- prescriptive(Decision opt./recommendation system),Generative(intelligent assistant,chat bots)
- work with unstructured data (text,images,videos,audio etc) eg.text based model(llm's)
- tool box has only one model (foundational model),scope :- wide (one model allow generalise to wide range of tasks )
- use case-->foundational model (pre-trained)-->prompt engineering(chaining prompts,parameter efficient fine-tuning(peft),retrival augmented generation(rag),agents)-->embedd

Data Scientist:-
- Data storytelling
- descriptive(clustring/EDA) and predictive(regression/classification)
- work mostly with structured data(tabular)
- there tool box contains(100's of models) having unique functionality,scope :- narrow (doesn't generalise)
- use case-->data-->preprocessing-->model-->deployment

## Why data is important for ML
- it is collection of raw facts, figures and information
- used to draw insights and information from data


## different types of ml tools
- store and retrieve data
- work with plots,graphs and dashboards
- explore,inspect and clean data
- prepare data
 eg:- Pandas library
 Scikit-Learn library

- types:-
- data processing and analytics :
-PostgreSQL(Relational database management system),Hadoop(Batch processing solution for big data),Spark(Distributed Data Processing),Apache-kafka(Distributed realt time streaming analytics),Pandas(Data wrangling and preprocessing),Numpy(Numerical computing)

- data visualization:- 
  visualize data (Matplotlib,seaborn,ggplot2,Tableau)
- Machine Learning:-
  Create and tune models (Numpy,Pandas,SciPy,Sci-kit learn)
- Deep Learning:- 
  Designing, training and testing neural network based models(Tensor Flow,Keras,Theano,Pytorch)
- Computer vision:-
  Object Detection,Image Detection,Facial Detection,Image segmentation,(libraries:- OpenCV,Scikit image,TorchVision)
- Natural Language processing:-
  help build application that generate, understand human language(NLTK,Textblob,Stanza)
- Generative Ai:- 
  leverage ai to generate new content based on input data (huggingface transformer,chatgpt,dall-e,pytorch)

### Scikit learn Ecosystem

## Machine learning ecosystem

it is a system that is interconnected with tools, frameworks,platforms that support building and deployment and managing ml models

## features and working of scikit learn library
all the basic machine learning pipeline can be done using scikit learn, like preprocessing,standardizing, model training, train test split, evaluations, transforming etc