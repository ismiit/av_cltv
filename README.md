# av_cltv

JOB-A-THON - JANUARY 2023.

Predicting the possible Customer Life Time Value given features of a customer in the dataset.

* The initial training data had 89392 data points and 11 features including the target feature 'cltv'.
* * EDA : We realised the following hints from EDA of the data 
* There were 9 categorical varibales out of which 7 were object type which were to be encoded into readable format for which I tried Target-Encoding and One-Hot encoding. One-Hot Encoding performed a lot better for variables : [ 'qualification', 'income', 'policy', 'type_of_policy']. While for variables I used basic Binary Encoding replacing a certain category with 1 while the other with 0.

       a. CLTV was highest for people with income <=2L.
       b. 
