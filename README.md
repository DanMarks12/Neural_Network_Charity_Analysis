# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis.
The purpose of our analysis was to use unsupervised deep learning neural networks alongside Tensorflow to provide analysis on an extremly large data set. The data set consisted of charity donations, and of those which were measured to have succes or not. This was done by first fixing our data to remove uneeded columns, getting our data ready for the neural network, compiling training and evaluating that model and lastly optimizing our model for best performance and results.

## Results: Using bulleted lists and images to support your answers, address the following questions.

## Data Preprocessing
### What variable(s) are considered the target(s) for your model?
We considered all variables for our analysis except columns EIN and NAME. We removed them because they contained identification information which is not pertinent for analysis. The main column used in analysis was IS_SUCCESFUL as it contained a binary answer which is useful for our depp learning neural network.
### What variable(s) are considered to be the features for your model?
![](https://github.com/DanMarks12/Neural_Network_Charity_Analysis/blob/main/JPG/FEATURES.JPG)
There were the features of the model: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
### What variable(s) are neither targets nor features, and should be removed from the input data?
As mentioned before EIN and NAME were removed as they were indentification information. 

## Compiling, Training, and Evaluating the Model
### How many neurons, layers, and activation functions did you select for your neural network model, and why?
In my neural network model I used two hidden layers with 80 and 30 neurons respectively. We used 25k samples. 
### Were you able to achieve the target model performance?
We only reached a model accuracy of 76% so we were not able to achieve the target model performance. We could more easily reach these numbers using more simple analysis methods.
### What steps did you take to try and increase model performance?
To further optimize our models performance we used the activation function RELU for hidden layers. We used Sigmoid on the output layer as it was a binary classification. To further improve our performance we used bucketing through ASK_AMT in order to change various values into intervals. I tried the analysis again with 3 neurons instead of 2 as well as another activation function: Tanhn. 


## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

As mentioned above we were not able to reach a useable level of accuracy in our model. At 76% we are able to predict the majority of donations correctly but not a meaningful amount to consider it useful. A problem like this may be more suited for work we used in past modules: SUPERVISED machine learning. The method I would suggest is the Random Forest Classifier as it closley emmulates the analysis we performed but we are able to control our inputs more carefully and then compare our results to ou rdeep learning model. 
