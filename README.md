# Predicting customer churn with Spark
Define what customer would churn from Sparkify's online services. The project uses pySpark to engineer features and to build classification model to predict churn.

![Predicting customer chrun](https://github.com/rabadzhiyski/SparkProject/blob/main/Sparkify_.png "Sparkify")

## Project Overview
Sparkify (a made-up company) provides online music services. With this project we developed a machine learning model to predict customer churn. The project uses pySpark libraries and it was developed with Jupyter notebooks developed on a local PC. A Spark cluster was also tested in [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio). There are three data sets available with customer data - mini, medium, and a 12GB data set. None of them are available in this repository due to their size. The project consists of:
- Jupyter Notebook - where all code is available
- [Blog post](https://medium.com/p/e7a4307870be/edit)
- Github repository - the present repository with all files and folders

## Problem Statement
Customer churn is a very challenging area and it gives many opporutnities for analyses. We use pySpark to load, transform data and build machine learning algorithm to predict Sparkify's users churn. It is important to find a way to get a realistic probability for users who are prompt to churn based on some features like gender, location, workday, songs played, etc. With the help of several pySpark libraries we will first explore the data, engineer the most appropriate features, deisgn a machine learning pipeline and choose the most approrpiate model for predicting churn. It is a classification task that will require Logistic Regression, Random Forest Classifier or other classification model.

## Metrics
To define if we worked correctly and we can count on our model we need some metrics. For this project we used area under ROC as a performance metric. Even if accuracy is a very popular metric, it's not the best choice for a binary classification problems who often produce unbalanced data. Like fraud, or spam filters, customer churn data of Sparkify has classes that are distributed unequally. For example,  when we run our logistic model it had remarquable accuracy of 99% but are under roc  = 65%. ROC (receiver operating curve) is the visual representation of performance of binary classifier. False Positive Rate vs True Positive Rate is plotted to get the visual understanding of the classifier's performance. 

## Conclusion 
As famous British statistician George Box stated "All models are wrong but some are useful". 
We should always link the models to the business context and make some assumptions about their use. For me, predicting churn was a challenging task and I would not say that our model is the best possible solution. However, it gave us a fresh inside and a reasonable confidence that with the right features, we can identify some Sparkify clients who are prompt to churn.

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
