# food-delivery-time-prediction-hackthon
Approach To Solving The Problem-

Steps:

1. Performed basic EDA 

2. Cleaned the data for numerical features like number of Ratings, Votes, Reviews, Average cost and Minimum order. Trained a Lightgbm model and was surprised to see that the model was not performing that well compared to logistic regression in the initial steps

3. Created few useful derived features like Minimum order to cost ratio, number of restaurants in a given location and number of branches of a given restaurant etc.

4. Determined the set of unique cuisines across all restaurants and created various cuisine features in a one hot encoded way.

5. Also the location information have multiple details in terms of area, city etc. but the details were not consistent and so created a feature City and mapped the Location to the cities accordingly.

6. Ensembled various models using geometric and harmonic mean. Tried ensembling various models like xgboost, lightgbm, random forest, logistic regression, etc. Finally selected Random Forest and Lightgbm and tuned them for final submission.

7. The Final submission was made based on ensemble of the Arithmetic mean of probabilities from lightgbm and random forest
