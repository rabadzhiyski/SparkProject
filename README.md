# Predicting customer churn with Spark
Define what customer would churn from Sparkify's online services. The project uses PySpark to engineer features and to build classification model to predict churn.

![Predicting customer chrun](https://github.com/rabadzhiyski/SparkProject/blob/main/Sparkify_.png "Sparkify")
*In case of troubles loading the .ipnb files wihtin Github, you can copy/paste the link of the document here: https://nbviewer.jupyter.org/*

**Attention:**
*Data sets were not added to the repository due to their size. The SparkifySpark version reads data from the cluster, adjustments might be needed if the code is tested: the correct path to the data sets should be entered in the df call!"*

## Project Overview
Sparkify (a made-up company) provides online music services. With this project we developed a machine learning model to predict customer churn. The project uses PySpark libraries and it was developed with Jupyter notebooks developed on a local PC. A Spark cluster was also used in [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio). There are three data sets available with customer data - mini, medium, and a 12GB data set. None of them are available in this repository due to their size. Mini version was used locally, and the medium-sized data was used in the cluster. The project consists of:
- Jupyter Notebook - where all code is available (working and final version)
- [Blog post](https://plamen-rabadzhiyski.medium.com/sparkify-make-your-customers-stay-e7a4307870be)
- Github repository - the present repository with all files and folders

## Problem Statement
Customer churn is a very challenging area and it gives many opporutnities for analyses. I used PySpark to load, transform data and build machine learning algorithm to predict Sparkify's users churn. It was important to find a way to get a realistic probability for users who are prompt to churn based on some features like gender, location, workday, songs played, etc. With the help of several PySpark libraries I explored the data, engineered the most appropriate features, deisgned a machine learning pipeline and chose the most approrpiate model for predicting churn. It is a classification task that required Logistic Regression, Random Forest Classifier or other classification model.

## Metrics
To define if I worked correctly and if we can count on our model I needed some metrics. For this project I used area under ROC as a performance metric. Even if accuracy is a very popular metric, it's not the best choice for a binary classification problems who often produce unbalanced data. Like fraud, or spam filters, customer churn data of Sparkify has classes that are distributed unequally. For example,  when we run our logistic model it had remarquable accuracy of 99% but area under roc  = 65%. ROC (receiver operating curve) is the visual representation of performance of binary classifier. False Positive Rate vs True Positive Rate is plotted to get the visual understanding of the classifier's performance. I tested boht but I chose Logistic regression over Random Forest as it was 23% more performant (0.65 vs 0.5)

## Conclusion 
As the famous British statistician George Box stated "All models are wrong but some are useful", we should not be over confident with the machine learning algorithms. We have to link the models to the business context and make some assumptions about their use. For me, predicting churn was a challenging task and I would not say that my model is the best possible solution. However, it gave me a fresh inside and a reasonable confidence that with the right features, I can identify some Sparkify clients who are prompt to churn.

## Content
The reposisotory contains all necessary documents (except the data sets):
- License
- Readme
- SparkifyDraft - working version of Jupyter notebook.
- SparkifySpark - final version of Jupyter notebook. Generated and used in the IBM Watson Studio.

## Libraries
Numpy, Pandas, MatplotLib, Seaborn, Plotly, Datetime, PySpark. 

## Acknowledgements
The project is part of the [Udacity Data Science Nanodegree program.](https://www.udacity.com/school-of-data-science)

## Reference documentation
- https://towardsdatascience.com/dealing-with-imbalanced-dataset-642a5f6ee297
- https://medium.com/@sarath13/area-under-the-roc-curve-explained-d056854d3815
- https://spark.apache.org/docs/1.5.2/
- https://www.kaggle.com/lpdataninja/machine-learning-with-apache-spark/notebook
- https://www.udacity.com/course/learn-spark-at-udacity--ud2002





