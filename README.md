# Conversion rate analysis
## I)Introduction
---
This is a sample project that can be used to help analyzing if a company is developed well, and giving convincing strategies along with the data 



## II)Getting Started
---
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.


- Prerequisites
    You will need a tool to run the program on your local machine such as:
    > VScode, Jupyter Note Book......

 
- Installing
    There are some packages that you will be using:
    > Pandas, Numpy, Matplotlib.pyplot, Seaborn, Scikit-learn(sklearn), bokeh, keras, pmdarima
    - Install packages on Jupyter NoteBook:
      > !pip install 'package name'


- Run the program
    The only thing you will need to do to run the test is input a CSV file with header 
    >[number, Name_of_currency, Symbo_of_currency, Date, High, Low, Open, Close, Volumn, Marketcap]


## III) Methodology
---
- Raw Data:
  
  I got the data from Kaggle, and you can also check for others' code as well. 


- Data pre-processing

Every time after getting a dataset, it is vital to do a quality check on the data to ensure the visulaization and modling sessions won't go wrong.
I started by using the describe funciton in Pandas and then check for any Null or missing values. After that, by uisng a heatmap, we could easily
observe the relationships among all the features. Another important step during data pre-processing is to remove outliers, which I used the IQR 
method here. 

- Data visualization
  
  In this part, I used line chart, histogram, heatmap, bar chats to get more insights from the data.

- Training Process:

Before training, we need to split the data into trainning and testing set, and in order to prevent overfitting, I left 30% of the data as testing set.
I used Logistic Regression, decision tree, and random forest, naive bayes here.


- Testing

  Each model has been tested on the test set. Besides,  I used AUC-ROC curve, test_accuracy, and confusion martirx to check the modeling result.


### model 1: Logistic regression:
  - From based line to gridSearchCV
  - train, test split
  - model Tunning
  - accuracy check

### model 2: random forest:
  - From based line to gridSearchCV
  - train, test split
  - model Tunning (tree depth, max split, etc.)
  - accuracy check





