# Predicting customer churn with Spark
Define what customer would churn from Sparkify's online services. The project uses pySpark to engineer features and to build classification model to predict churn.

Add image

## Project Overview
Sparkify (a made-up company) provides online music services. With this project we developed a machine learning model to predict customer churn. The project uses pySpark libraries and it was developed with Jupyter notebooks developed on a local PC. A Spark cluster was also tested in [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio). There are three data sets available with customer data - mini, medium, and a 12GB data set. None of them are available in this repository due to their size. The project consists of:
- Jupyter Notebook - where all code is available
- [Blog post](https://medium.com/p/e7a4307870be/edit)
- Github repository - the present repository with all files and folders

## Problem Statement
Customer churn is a very challenging area and it gives many opporutnities for analyses. We use pySpark to load, transform data and build machine learning algorithm to predict Sparkify's users churn. It is important to find a way to get a realistic probability for users who are prompt to churn based on some features like gender, location, workday, songs played, etc. With the help of several pySpark libraries we will first explore the data, engineer the most appropriate features, deisgn a machine learning pipeline and choose the most approrpiate model for predicting churn. It is a classification task that will require Logistic Regression, Random Forest Classifier or other classification model.

## Metrics
To define if we worked correctly and we can count on our model we need some metrics. For this project we used F1 score, and confusion metrics to define the best model. We would consider appropriate a model with F1 socre of (TBC).

## Content
The reposisotory contains all necessary documents (except the data sets):
- License
- Readme
- SparkifyDraft - working version of Jupyter notebook
- Sparkify - final version of Jupyter notebook

## Libraries
Numpy, Pandas, MatplotLib, Plotly, Datetime, Pyspark, 

## Acknowledgements
The project is part of the Udacity Data Science Nanodegree program. 
