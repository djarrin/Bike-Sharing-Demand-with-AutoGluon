# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### David Jarrin

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The main change I needed to make when submitting my results to Kaggle was that I needed to only
include the datetime and the count columns

### What was the top ranked model that performed?
My top ranked model was the one where I kept most of the defaults for the AutoGluon model but added in the hours feature. I believe in my 3rd model
where I was doing the hyperparameter turning I added more time for the model to train and switched on the auto_stack parameter, this didn't perform as well for one of two reasons (I think); I think adding
more time to the model may have led to over fitting or the 2nd possibility is adding the auto_stack parameter required for the model to train for longer and perhaps if I would have increased the time_limit parameter
I would have seen better results.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I noticed a regular pattern once I graphed the hours feature so I added that into what to train against.

### How much better did your model preform after adding additional features and why do you think that is?
The model preformed significantly better with a score difference of 3.963232999999999. This most likely improved results because it gave the model time of day during the which part of the year
people were normally riding bikes (winter has fewer day light hours).

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
It actually performed slightly worse with the parameters I added in.

### If you were given more time with this dataset, where do you think you would spend more time?
I would spend more time adjusting the parameters to see if I could get the Kaggle scores down.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
Please see worksheet for this table (towards the bottom)

### Create a line plot showing the top model score for the three (or more) training runs during the project.

![model_train_score.png](https://github.com/djarrin/Bike-Sharing-Demand-with-AutoGluon/assets/7516512/92c54e87-5ef9-4d07-8dbd-d4fe4cb28b5a)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

![model_test_score.png](https://github.com/djarrin/Bike-Sharing-Demand-with-AutoGluon/assets/7516512/fcad3bb8-e6f5-41f7-ada6-d9659317a55b)

## Summary
This was an informative project where I became more familiar with SageMaker studio and the AutoGluon tool. I was able to achieve the best 
results relatively quickly by using defaults of AutoGluon and adding in features for Exploratory Analysis.
