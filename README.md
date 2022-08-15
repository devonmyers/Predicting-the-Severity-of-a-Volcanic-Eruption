# Predicting-the-Severity-of-a-Volcanic-Eruption
I have designed a machine learning model capable of predicting the Volcanic Explosivity Index (VEI) using XGBoosted Trees for multiclass classificaiton.
The outcome variable dataset for this project has an imbalance among its levels and some of the input features have missing data.  
To handle the imbalance in the outcome varible, I employ a simple oversampling technique to ensure that each outcome class has the same number of observations.
Missing data was imputed using JMP 14.
JMP 14 was also used for visualization tasks.
Additionally, to compute accuracy, I employ a one-off accuracy metric.
This one-off accuracy allows a predicted value to be considered 'correct' if it is within one unit of the true outcome.
The thought process behind one-off accuracy is that if my model predicts a volcanic eruption will be a 5.0, and it turns out that the actual eruption is 4.0, it is not that far off the mark.
Basically, if the model predicts a bad enough eruption (i.e. 3.0 or higher), it is probably a good idea to pack things up and evacuate!

Data exploration was carried out using both JMP 14 for visualization and also Python code found in the VolcanoEruptionAnalysis.ipynp.
The .ipynp file called XGBoostVolcanoModel contains code to run the VEI predictor.
This model relies on imputed data and oversampling to handle imbalance in VEI.
To run the VEI predictor, simply download the .ipynp file mentioned previously,  and also the merged_info_volcanoes.csv file.
