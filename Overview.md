# deep-learning-challenge

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Overview of the Analysis The purpose of this analysis is to develop a deep learning model using TensorFlow to predict whether an organization funded by Alphabet Soup will be successful based on a set of features. The model aims to achieve 75% predictive accuracy.

Results: Using bulleted lists and images to support your answers, address the following questions:

What variable(s) are the target(s) for your model?
> IS_SUCCESSFUL is the target variable, reflecting if funded organization was successful.


What variable(s) are the features for your model?
> Below variable where encoded to convert them into binary except ask_amt which is not categorical
APPLICATION_TYPE	9
AFFILIATION	6
CLASSIFICATION	6
USE_CASE	5
ORGANIZATION	4
STATUS	2
INCOME_AMT	9
SPECIAL_CONSIDERATIONS	2
ASK_AMT	8747
IS_SUCCESSFUL	2

What variable(s) should be removed from the input data because they are neither targets nor features?
Compiling, Training, and Evaluating the Model
> Two columns were removed EIN, and name as it has no role in the success of an organization

How many neurons, layers, and activation functions did you select for your neural network model, and why?
> Used 2 hidden layerss and later on added another two more layers to increase the accuracy of the model, Total 4 hidden layers. The first first hidden layer started with 30 neurons but made it to 80 neurons to the first hidden layer to increase accuracy. 

Were you able to achieve the target model performance?
> Despite trying multiple time the target model accuracy of 75% was not acheived

What steps did you take in your attempts to increase model performance?
> Used 2 hidden layerss and later on added another two more layers to increase the accuracy of the model, Total 4 hidden layers. The first first hidden layer started with 30 neurons but made it to 80 neurons to the first hidden layer to increase accuracy.Also increased the number of epochs to 200 and changed kernel_regularizer l2 to 0.0001 from 0.01.
Despite all the changes the model did  not achieved target accuracy.


Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

>The Model achieved accuracy of 73% and hit a pleateau beyond a point. May be using other model like GBM could help