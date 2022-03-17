# Amazon comments classifier: Project Overview

This proyect use ML models to classifie comments of prodcuts on Amazon as good, bad or neutral

-I Created a machine learning model to classifie comments. The comments are linked to  a rating made by the same user from 1 to 5

-This is a problem of classification. The classification models used are: logistic regression and Random Forest


# Code and Resources Used
 
Python Version: 3.10

**Packages**: pandas, numpy, matplotlib, seaborn, re, sklearn, nltk
 

# Samplig and data cleaning

Fist a i made data cleaning, dropping NA values.

I took 20% of the data frame, the values were choosen in  a random way. This step was neccesary due to the size of the original data frame.

looking at the date we see that there is an obvious inbalance of the data towards the 5. So i Made a compensation with value with less number of entries.

After that i used a world lemmatizer and regular espressions to clean the comments of unnecesay characters, in order to help the model to make a better calification.


# Test and training

Before start writting the code for the actual model, i made a bag of words and vectorization of the values

Then i divided the sample in two groups: test and training

# Classification

I used two models from Scikitlearn: Logistic regression and Random Forest Classifier.

# Evaluation
The f1_score gave a result of 0.5879106438896189
[0.59920058 0.51109215 0.64717582]

The Confusion_matrix, the classification_report and the accuracy_score gave me similar values

I tried to tune the model, but the results continued to be negative, with scores around .6 always in both models.
