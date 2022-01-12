# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
Results of predictions were based on hyperparameters used and how results get optimized after chnaging values from default to trying out different values.

### What was the top ranked model that performed?
Creating additional features and hyperparameters gave me better results. 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I did EDA with visualizing data using time attribute. In hour data got inference that in morning bike sharing increases. On weekends afternoon bike sharing increases.
Then I did correlation matrix analysis. I found high correlation in target matrix and casual, registered. Temperature was also somewhat correlated. But humidity parameter was not affecting overall target matrix. So overall season, weather and temperature seems like affecting factors. 

### How much better did your model preform after adding additional features and why do you think that is?
Model score improved by 5% after adding hyperparameter. Adding extra features and using hyperparameters helped me improve model score.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
After using different hyperparameters my model score improved from 0.57 to 0.46 i.e. by 19%.

### If you were given more time with this dataset, where do you think you would spend more time?
I would try different algorithms like xgboost and different regression algorithms. And trying different algorithms which improves score.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|time|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|--|
|initial|600|Default Values|Default Values|Default Values|1.38964|
|add_features|600|Default Values|Default Values|Default Values|0.48265|
|hpo|1500|GBM|NN|num_bag_folds=5, num_bag_sets=1, num_stack_levels=1|0.51059|
    
### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](nd009t-c1-intro-to-ml-project-starter/model_train_score.png)
![train](https://user-images.githubusercontent.com/96059146/149206899-07407867-228c-45e3-a1ae-60c6f20eb4ed.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](nd009t-c1-intro-to-ml-project-starter/model_test_score.png)
![test](https://user-images.githubusercontent.com/96059146/149206807-f463d44e-c9ea-404e-8fa2-50893c9e8947.png)

## Summary
Final inference is kaggle score improved by using hyperparameters and adding extra features.
