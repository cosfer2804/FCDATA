![alt text](https://github.com/cosfer2804/FCDATA/blob/main/logo.png)

# IRONHACK MID THERM PROJECT: BANK CASE STUDY

BY FC DATA (Thiago and Angela)

### Table of Contents
* Scenario
* Objective
* Tools and methods
* Business insight

## Scenario
You are working as a risk analyst with a bank. The bank provides credit card services and wants to understand the demographics and other characteristics of its customers that accept a credit card offer and that do not accept a credit card.

## Objective
* Build a model to predict which customers are likely to accept an offer.
* Identify the demographics and charateristics which most influence whether a credit card offer is accepted or rejected.

## Tools and methods

* Trello - using agile method (Kanban)

* MySQL

* [Tableau] (https://public.tableau.com/app/profile/angela6850/viz/FCdataclassification/Dashboard?publish=yes)

*  [Python](https://www.python.org/)
* #### Initial cleaning steps   
  deal with nulls and drop useless columns
* #### EDA
  review columns' distribution, counts and correlation
* #### Pre-processing: encode categories and scale numerics
* #### Train, test, split
* #### Define model
  Logistic regression classify
* #### Check accuracy of our classification model
* #### Fit the model to more balanced data
* #### Resampling techniques
  confusion_matrix and heatmap
* #### Correlating categories
  Random Under Sampler and Random Over Sampler
* #### AUC

### 1. Explore the data
To explore the data, you can use the techniques that have been discussed in class. Some of them include using the describe method, checking null values, using Matplotlib, and Seaborn for developing visualizations.

The data has many categorical and numerical variables. Explore the nature of data for these variables before you start with the data cleaning process and then data pre-processing (scaling numerical variables and encoding categorical variables).

For the target variable (Offer accepted – Yes/No), it is also an important to check the data imbalance ie., the number of people who responded with a yes vs. the number of people who responded with a no.

### 2. Build a Model
Use different models to compare the accuracies and find the model that best fits your data. You can use the measures of accuracies that have been discussed in class. Please note that while comparing different models, make sure you use the same measure of accuracy as a benchmark.

### 3. Visualize
You will also use Tableau to further visually explore the data. You will deep dive in the data for customers who accepted the offer vs the customers who did not and check their characteristics. E.g., we select the Yes level in Offer Accepted and then examine the distribution of accepted offers across the other variables in our data set and similarly for people who did not accept the offer.

## Deliverables
A slides deck: use slides.com for simple yet effective templates.
A presentation: Your public presentation should last between 5 and 7 minutes.
SQL Queries: Access the SQL Questions file and make sure you run these queries using SQL.
A Tableau Dashboard: Follow the instructions in this file to build in Tableau.
Python code: Your code will be reviewed. Make sure you follow the best practices explained in class so far.
Evaluation criteria
Critical Thinking
Communication
Transparency
Thoroughness
Rubrics
These are the rubrics we use to assess your work.

## Tips & Tricks
Organize yourself (don’t get lost!). Respect deadlines.
Ask for help but don’t forget that Google is your friend.
Define a simple approach first. You never know how the data can betray you. :wink:
Document your work.
Learn about the problem and what research has been done before you.
Before making a graph, think about what you want to represent.
