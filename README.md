# Data Science Project #1 - Investigating a Financial Data Set of Loans.

## The Dataset
For this project, I as using a public dataset from Kaggle located here: 
https://www.kaggle.com/datasets/gauravduttakiit/loan-defaulter

## Acknowledgements 
The name of the person posting the dataset (listed above) from Kaggle that I am using is Gaurav Dutta. 


## Motivation
The motivation for this study was for 2 reasons. The first was to fill a requirement for a Udacity course. The second is that I work in finance and find it interesting as a field. 
This dataset looks pretty well organized with many features. This, combined with the type of data (financial) made it interesting to me. 


## Files Used
There are 3 files in this data set.
1) "columns_descriptions.csv" -- a file describing the column names and descriptions
2) "application_data.csv" -- the main data showing contract information on a set of over 300K contracts with a target variable indicating whether or not a particular customer was classified as having trouble paying back a loan along with many feature variables.
3) "previous_application.csv" -- a file with information about past applications for customers. NOTE: for this project I am not using this file because it does not have previous payment history and it is also very large, affecting performance. In addition, there are many fields in the main data that we can utilize for an initial study. 


## Python Libraries Used
pandas, 
numpy,
sklearn, 
scipy,
matplotlib


## Questions Asked
Looking at the data I asked a few questions: 
1) What is the percent of contracts that had challenges repaying the loan?
2) What type of machine learning model would be a good choice to use?
3) Does the amount of the loan relative to a party's income (whether an individual or corporate entity) have an effect on the default rate? NOTE: this is not a variable in the data. 
4) What other variables would the model consider important? Can we gain any insights from this? 


## Method
To answer these questions, I am utilizing python to do machine learning. I am using python version 3.8

I used 2 models concurrently to see which one, if either, would perform better - a logistic regression model and also a random forest classifier model. Both had very close accuracy rates of about 87%. The random forest model had slightly higher accuracy so I used that model to assist in answering questions. 


## Summary
The odds of challenges to repaying the loan were 13% overall. 

Classification was the way to go as far as what kind of machine learning since we are trying to predict a yes no question. That question being: is the customer likely to pay back the loan or no? 

The amount of the loan relative to a party's income was an important variable according to the model, but not the most important one. The most important variable was an external normalized data source that has characteristics of a credit bureau's data. 

2 other variables that were some of the more important ones were the age of a customer and how many days they had their current cell phone. 

To see more details, please reference the jupyter notebook in this repo. Thanks! 

 



