# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Syeda Laiba Azam

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: I was needed to remove negative values since it is not allowed to have negative prediction to be submitted in kaggle competition

### What was the top ranked model that performed?
TODO: WeightedEnsemble_L3 with added feature was the top ranked model that performed with the validation score of 30.220693 .

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: 
We changed the season and weather column into category type since they were categorical data,also we added  new column oarse by parsing datetime feature and this two changes significantly improved performance  
### How much better did your model preform after adding additional features and why do you think that is?
TODO: Initial the score was 52.816116 and after adding feature it went to 30.220693 hence the improvement is quite evidant and I think it is because we changed season and weather feature into  category that were previously read as integer datatype .

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: the kaggle score was increased indeed after hyperparameters tuning .the RMSE was better than the initial model result but the score of after features being added is still at the top in terms of performance 

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: I will expand more time in data preprocessing becuase i think we are training usng too many features .I would have explored feature reduction possibilities.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|

|initial|default|default|default|1.80214|
|add_features|default|default|default|0.67826|
|hpo|gbm|knn|rf|0.50664|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.


!Predict-Bike-Sharing-Demand-with-AutoGluon/project/img/model_train_score.png

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

!Predict-Bike-Sharing-Demand-with-AutoGluon/project/model_test_score.png

## Summary
TODO: in term of RSME score the model with added feature performed well with a score of 30.220693 whereas kaggle score of model with hyper parameter tuning showed better performance with the score of  0.50664.

