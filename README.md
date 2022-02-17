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

### Trello - using agile method (Kanban)

### Github

### MySQL

### [Tableau](https://public.tableau.com/app/profile/angela6850/viz/FCdataclassification/Dashboard?publish=yes)
* Visualize and deep dive in the data to find customer behaviour patterns

### [Python](https://www.python.org/)
* #### Deal with nulls, check duplicates and drop useless columns
* #### EDA - review columns' distribution, counts and correlation
* #### Visualizations - Matplotlib and Seaborn to check if there are outliers
* #### Pre-processing: encode categories and scale numerics

* #### Train, test, split

* #### Define model
  Logistic regression classify
* #### Check accuracy of our classification model
* #### Fit the model to more balanced data
* #### Resampling techniques confusion_matrix and heatmap
* #### Correlating categories
  Random Under Sampler and Random Over Sampler
* #### AUC

### Model Result
Use different models to compare the accuracies and find the model that best fits your data. You can use the measures of accuracies that have been discussed in class. Please note that while comparing different models, make sure you use the same measure of accuracy as a benchmark.

### Insight
* We have the most offer accepted during Q2 and Q3.
* The average balance increases esponentially from Q1 to Q3 in category A, while it  remains invariate in category D. Categories B and C have a linear average balance   grow from Q1 to Q3 and drop from Q3 to Q4.
* 62% of the clients that accepted the offer has low credit rating, followed by 26%  with medium creadit rating and only 12% with high credit rating.
* It seems that there is a preference in receiving the offer through postcard in the group who accepted the offer.

### Next steps
To further deep dive into the study we might need some more demographic (age) and geographic (residence) information about the target. For istance, in some countries, people tend to go to holidays during Q2 and Q3, so therefore more money are kept in the bank account. Also, during holidays, people might need a credit card?
