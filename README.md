# Neural_Network_Charity_Analysis
Module 19 Challenge

## Overview 
Using neural network analysis, design and train a deep learning neural network that effectively classifies a donation as being successful to inform future donation decisions. We used the Python TensorFlow library to develop this neural network.

## Results: 

### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
- The binary classifcation "IS_SUCCESSFUL" is the model target
#### What variable(s) are considered to be the features for your model?
- Varibles included in the analysis were Application Type, Affiliation, Classification, Use Case, Organization Type, Status, Income Amount, Special Considerations, and Ask Amount
#### What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN and Name were removed from the input data

### Compiling, Training, and Evaluating the Model
#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
- The initial model included two hidden layers, with 80 neurons in the first and 30 in the second. There was also an output layer.
- Activation functions used for the hidden layers were "relu" and "sigmoid" was used for the ouptut layer.
- The "sigmoid" function presents a binary outcome between 0 and 1, a helpful result when attempting to classify a charitable donation and successful or not.

#### Were you able to achieve the target model performance?
- No, the model only achieved 72.5% accuracy.

#### What steps did you take to try and increase model performance?
- Re-binned the APPLICATION_TYPE to group all with counts <1000 compared to the original model that grouped those with <500
- Added a third hidden layer with 20 neurons
- Converted the outputlayer to use a "tanh" function instead of a "sigmoid" function

## Summary: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
- Remove Status
- Bin Ask Amount
