### Models

To perform each model, we developed a for loop in which we applied Logistic Regression, Random Forest, KNeighbors and Gradient Boosting to the same dataframe. In this way, it was possible to compare and evaluate which methods obtained the best results.

So after testing nine different models, we decided to give attention to two of them that had a more relevant result. It is worth noting that each model represents two different marketing strategies. 

#### Model 1 - Logistic Regression (using SMOTE for resampling)
Despite achieving only 69.6% accuracy, this model is the most ideal for implementing a marketing strategy that will focus on potential customers without losing those who have already accepted the offer. 
When we evaluate the confusion matrix, it is possible to notice that the model predicts 5.6% of true positives from the total number of customers, which corresponds to more than 90% of the customers who accepted the offer. On the other hand, we notice that the model predicts 30% false positives. However, in our case false positives are considered as possible customers. This way, we can use this model to design a marketing strategy to keep most of the customers that have already accepted the proposal and make new offers to potential customers. 
It is worth noting that the model only made statistical evaluations. Therefore, if there is any interest in implementing this strategy, financial planning is required to assess its viability.

<img width="400" alt="https://github.com/cosfer2804/FCDATA/blob/main/screenshot/knn_best1.png">

#### Model 2 - Random Forest (using Smote and Tomek Links for sampling)
Model 2 had 87.2% accuracy, but in relation to the confusion matrix the efficiency was lower than model 1. It can be stated that this model lost 2% of the customers who already accepted the proposal (comparing to the previous model), and predicted 10.6% of potential customers. In this situation, the bank can use this model to develop a strategy for a low operational cost. Despite the fact that this model is not as efficient, it may have a much higher viability than model 1.

<img width="400" alt="Random Forest" src="https://github.com/cosfer2804/FCDATA/blob/main/screenshot/randomforest_best2.png">

## Next Steps

To further progress this study and increase the accuracy of both models, it would be useful to collect more demographic information on the customers such as maritial status or employment status. Furthermore, knowing more about which customers live in the same residence by having a household_id would be helpful to further refine our 'capita' column. Lastly, having specific information on customers' income we think would greatly benefit the models.
