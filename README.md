# av_cltv

JOB-A-THON - JANUARY 2023.

Predicting the possible Customer Life Time Value, given features of a customer in the dataset.

* **The initial training data had 89392 data points and 11 features including the target feature 'cltv'.**
* **EDA : We realised the following hints from EDA of the data 
 
       a. CLTV was highest for people with income <=2L.
       b. Customers with current policy 'C' bear higher CLTV.
       c. 'Platinum' policy also suggests higher CLTV values.
       d. 'Claim Amount' and 'cltv' both are rightly skewed.
       
* **Feature Encoding : There were 9 categorical varibales out of which 7 were object type which were to be encoded into readable format for which I tried Target-Encoding and One-Hot encoding.

       a. One-Hot Encoding performed a lot better for variables : [ 'qualification', 'income', 'policy', 'type_of_policy']. 
       b. While for variables I used basic Binary Encoding replacing a certain category with 1 while the other with 0.

* **Feature Importance : On evaluating the feature importance , it was found that num_policies and claim amount were the most effectable features.
* ** Model Making : 

      a. Creating a train and validation set with 80%-20% split.
      b. Scaling : Used RobustScaler and Standard Scaler but got better results with Robust Scaler.
      c. Defining a function that would evaluate the best possible Model out of LinearRegression,Lasso,Ridge,RandomForest,DecisionTree,AdaBoost,GradientBoost,CatBoost.
      d. The GradientBoost Regressor gives the best r2 score. The next challenge is to improve the data for better r2 scores.
 
 * **Feature Engineering
 
    a. Creating a new feature 'cust_type' that is created using clustering similar type of customers into two clusters based on the existing features.

