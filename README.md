# Predicting-the-Severity-of-a-Volcanic-Eruption
I have designed a machine learning model capable of predicting the Volcanic Explosivity Index (VEI) using XGBoosted Trees for multiclass classificaiton.
The outcome variable dataset for this project, VEI, is quite imbalanced.  
To handle this imbalance in the outcome varible, I employ a simple oversampling technique to ensure that each outcome class has the same number of observations.
Additionally, I employ a one-off accuracy metric.
This one-off accuracy allows a predicted value to be considered 'correct' if it is within one unit of the true outcome.
The thought process behind one-off accuracy is that if my model predicts a volcanic eruption will be a 5.0, and it turns out that the actual eruption is 4.0, it is not that far off the mark.
Basically, if the model predicts a bad enough eruption (i.e. 3.0 or higher), it is probably a good idea to pack things up and evacuate!
