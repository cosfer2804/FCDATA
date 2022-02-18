![alt text](https://github.com/cosfer2804/FCDATA/blob/main/screenshot/logo.png)

# MID PROJECT - CLASSIFICATION BANK CASE STUDY

BY Thiago Costa and Angela Wang

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

### [Trello](https://trello.com/b/I8S3Yl00/fc-data) 
* Using agile method (Kanban)

### [Github](https://github.com/cosfer2804/FCDATA)

### MySQL

### [Tableau](https://public.tableau.com/app/profile/angela6850/viz/FCdataclassification/Dashboard?publish=yes)
* Visualize and deep dive in the data to find customer behaviour patterns

### [Python](https://www.python.org/)
* #### EDA 
* #### Visualizations - Seaborn to check data distribution and outliers
* #### Pre-processing: encode categories and scale numerics with dummies
* #### Correlating categories using Chi square
* #### Models Logistic Regression, Random Forest, KNeighbors and Gradient Boosting
* #### Fit the model to more balanced data using resampling techniques Smote and Tomelink and visualize with confusion_matrix and heatmap

### Models

To run each model, We developed a for loop function that apply Logistic Regression, Random Forest, KNeighbors and Gradient Boosting to the same dataframe allowing us to compare and evaluate which methods had the best results simultaneously.

After testing nine different models, we selected the two following models with some interesting results that can be choosen depending on the company marketing strategy.

#### Model 1 - KNeighbors (using SMOTE for resampling)
Despite achieving only 69.6% accuracy, this model is the most ideal for implementing a marketing strategy that will focus on potential customers without losing those who have already accepted the offer. 

When we evaluate the confusion matrix, it is possible to notice that the model predicts 5.6% of true positives from the total number of customers, which corresponds to more than 90% of the customers who accepted the offer. On the other hand, we notice that the model predicts 30% of false positives. However, in our case, false positives are considered as possible customers. This way, we can use this model to design a marketing strategy to keep most of the customers that have already accepted the proposal and make new offers to potential customers. 

It is worth noting that the model only made statistical evaluations. Therefore, if there is any interest in implementing this strategy, financial planning is required to assess its viability.

<img width="400" alt="KNeighbors" src="https://github.com/cosfer2804/FCDATA/blob/main/screenshot/knn_best1.png">

#### Model 2 - Random Forest (using SMOTE for resampling)
Model 2 had 87.2% accuracy, but in relation to the confusion matrix the efficiency was lower than model 1. It can be stated that this model lost 2% of the customers who already accepted the proposal (comparing to the previous model), and predicted 10.6% of potential customers. In this situation, the bank can use this model to develop a strategy for a low operational cost. Despite the fact that this model is not as efficient, it may have a much higher viability than model 1.

<img width="400" alt="Random Forest" src="https://github.com/cosfer2804/FCDATA/blob/main/screenshot/randomforest_best2.png">

### Insight
* We have the most offer accepted during Q2 and Q3.
* The average balance increases esponentially from Q1 to Q3 in category A, while it remains invariate in category D. Categories B and C have a linear average balance   grow from Q1 to Q3 and drop from Q3 to Q4.
* 62% of the clients that accepted the offer has low credit rating, followed by 26%  with medium creadit rating and only 12% with high credit rating.
* It seems that there is a preference in receiving the offer through postcard in the group who accepted the offer.

### Next steps
To further deep dive into the study we might need some more demographic (age) and geographic (residence) information about the target. For istance, in some countries, people tend to go to holidays during Q2 and Q3, so therefore more money are kept in the bank account. Also, during holidays, people might need a credit card?
