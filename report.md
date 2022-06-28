# Report

## Overview of the analysis
The goal of the analysis is to, given the provided dataset, create a binary classifier that predicts whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

 * *What variable(s) are considered the target(s) for your model?*


   The feature named IS_SUCCESSFUL is the target of our model

 * *What variable(s) are considered to be the features for your model?*

    All other fetures: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT' except 'EIN' and 'NAME'

 * *What variable(s) are neither targets nor features, and should be removed from the input data?*

    'EIN' and 'NAME' 
### Compiling, Training, and Evaluating the Model
 * *How many neurons, layers, and activation functions did you select for your neural network model, and why?*
  
  I tried multiple configurations - please refer to the notebooks. I have tried to maintain roughtly 2 to 3 times the number of input features and have decided on the number of hidden layers by observing whether the model overfits.
 * *Were you able to achieve the target model performance?*

No, 75% was my best score

 * *What steps did you take to try and increase model performance?*
  
    - Dropping features based in observing correlations with the target variable through EDA plots
    - Adding hidden layers
    - Adding neurons to each hidden layer
    - Changing the batch size
    - Changing the activation function
    - Change in the bining

## Summary

There were multiple NN models that seemed to perfor similarly, *i.e.* ~73% accuracy. After exploration, the multiple feature engineering attempts (removing features or changing categorical binning) or the model fine tuning (batch size, number of neuros, activation function, etc.) didn't seem to significantly affect the performance on the test dataset
