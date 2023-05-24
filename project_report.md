# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### David Jarrin

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The main change I needed to make when submitting my results to Kaggle was that I needed to only
include the datetime and the count columns

### What was the top ranked model that performed?
My top performing model was my 3rd and final model (with the hyperparameter tuning). This honestly was a little bit of a surprise to me as in my first
submission this method performed worse and it seems this isn't the most efficient way to use AutoGluon. I believe this was a little bit of luck in picking the correct parameters
to tune and then focusing more training time just on those parameters (also I wasn't using the hyperparameter and hyperparameter_tune_kwargs correctly the first submission).

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I noticed a regular pattern once I graphed the hours feature so I added that into what to train against.

### How much better did your model preform after adding additional features and why do you think that is?
The model preformed significantly better with a score difference of 3.963232999999999. This most likely improved results because it gave the model time of day during the which part of the year
people were normally riding bikes (winter has fewer day light hours).

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
I increased my Kaggle score by 0.1836.

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
