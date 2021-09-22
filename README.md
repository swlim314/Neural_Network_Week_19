# Neural Network Analysis
## Overview of Analysis
The goal of this analysis is to determine whether candidates will be sucessful if funded by Alphabet Soup. A csv was provided of over 34,000 applicants with information on each
of those organizations as follows:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

This data was preproccessed to prepare for the training and running of a neural network analysis. After that was completed, several optimizations were attempted to push the target
predictive accuracy higher. 

## Results
For Data Preprocessing:
1. What variable(s) are considered the target(s) for your model? Based on the columns provided in the CSV, the target variable that would indicate sucess is the "IS_SUCCESSFUL"
column, which shows if the money was used effectively.
2. What variable(s) are considered to be the features for your model? All the other provided variables/columns would be considered the features for the model.
3. What variable(s) are neither targets nor features, and should be removed from the input data? Based on the pre-processing completed during the first deliverable, EIN and NAME
serve solely to be identification columns, and would not be needed in the neural network model. 

Compiling, Training, and Evaluating the Model:
1. How many neurons, layers, and activation functions did you select for your neural network model, and why? For the original neural network model, there were two hidden layers,
with there first layer having 80 neurons, and the second layer having 30 neurons. The activation functions were both relu.
2. Were you able to achieve the target model performance? With the original model, it was only able to hit a 72.9% accuracy.
3. What steps did you take to try and increase model performance? Below are three images of changes made to the neural network in an attempt increase the model performance. I
was unable to increase the model performance to hit the 75% requirement.


![AlphabetSoupCharity_Optimization1](https://github.com/swlim314/Neural_Network_Week_19/blob/538fe9b7930aa0f2ac9926508873ff792a4ab705/AlphabetSoupCharity_Optimization1.png)

![AlphabetSoupCharity_Optimization2](https://github.com/swlim314/Neural_Network_Week_19/blob/538fe9b7930aa0f2ac9926508873ff792a4ab705/AlphabetSoupCharity_Optimization2.png)

![AlphabetSoupCharity_Optimization3](https://github.com/swlim314/Neural_Network_Week_19/blob/538fe9b7930aa0f2ac9926508873ff792a4ab705/AlphabetSoupCharity_Optimization3.png)


## Summary
Overall the original neural network was very close to that 75% requirement. With a few more optimization, the predictive accuracy could have been increased to give a better idea
of what organizations would be well suited to be funded by Alphabet Soup. It might be simpler to use a linear regression model to avoid overfitting the data, with an assumption
that the data is more better suited to linear relationships.
