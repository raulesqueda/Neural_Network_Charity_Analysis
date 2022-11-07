# Neural_Network_Charity_Analysis

# Module 19 Challenge

## Overview of the analysis

After learning about neural networks, now we been assigned to help a foundation to predict where we could invest. For this, we support Beks to use machine learning and neural networks and create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

This database has more than 34,000 organizations DATA that have received funding from Alphabet Soup over the years. this dataset contains the following information:
1.	EIN and NAME—Identification columns
2.	APPLICATION_TYPE—Alphabet Soup application type
3.	AFFILIATION—Affiliated sector of industry
4.	CLASSIFICATION—Government organization classification
5.	USE_CASE—Use case for funding
6.	ORGANIZATION—Organization type
7.	STATUS—Active status
8.	INCOME_AMT—Income classification
9.	SPECIAL_CONSIDERATIONS—Special consideration for application
10.	ASK_AMT—Funding amount requested
11.	IS_SUCCESSFUL—Was the money used effectively

We were task to do three technical analysis deliverables and a report for the investment results.

## Results

Using our knowledge, we start processing the dataset to compile, train, and evaluate the neural network model for this purpose, we need answer the following questions:
**What variable(s) are considered the target(s) for your model?**
We considered as target variable for our model the one called “IS_SUCCESSFUL”.

**What variable(s) are considered to be the features for your model?**
As features, we considered the variables “APPLICATION_TYPE”, “AFFILIATION”, “CLASSIFICATION”, “USE_CASE”, “ORGANIZATION”, “STATUS”, “INCOME_AMT”, “SPECIAL_CONSIDERATIONS” and “ASK_AMT”.           

**What variable(s) are neither targets nor features, and should be removed from the input data?**
The variables we considered to be removed from the data where “EIN” and “NAME”.

### Compiling, Training, and Evaluating the Model

After processing and analyzing the data, we proceed to compiling, training, and evaluating the model, resulting the next model:

![Grafica1](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica1.PNG) 

**How many neurons, layers, and activation functions did you select for your neural network model, and why?** 
For the neural network model, we use 2 hidden layers with 80 neurons and 30, for both hidden layers we use the "relu" activation function and the output layer has the "sigmoid" activation function.

**Were you able to achieve the target model performance?**
Unfortunately, this model was not able to reach the target 75% of accuracy, the accuracy for my model was 72.71%.

![Grafica2](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica2.PNG) 
 
**What steps did you take to try and increase model performance?**

To achieve the target of 75% of accuracy of the model, we develop three neural network models with different specifications. In the first, we use 2 hidden layers with 40 neurons and 20, for both hidden layers we use the "relu" activation function and the output layer has the "sigmoid" activation function:

![Grafica3](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica3.PNG) 
 
The accuracy was better in comparison with the previous model, the accuracy results int 72.38%, but we didn’t reach the target.

![Grafica4](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica4.PNG) 
 
For the next attempt, we use 3 hidden layers with 50, 25 and 15 neurons, for both hidden layers we use the "relu" activation function and the output layer has the "sigmoid" activation function:

![Grafica5](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica5.PNG) 
 
We got a better result for the accuracy, although, the accuracy results int 72.59%, again, this model didn’t reach the target.

![Grafica6](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica6.PNG) 
 
For the last attempt, we use 3 hidden layers with 60, 30 and 20 neurons, for both hidden layers we use the "relu" activation function and the output layer has the "sigmoid" activation function:

![Grafica7](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica7.PNG) 
 
This model has the worst accuracy with 71.95%, this model didn’t reach the target.

![Grafica8](https://github.com/raulesqueda/Neural_Network_Charity_Analysis/blob/main/Gr%C3%A1ficas/grafica8.PNG) 
 
## Summary

The estimated neural network models we develop couldn’t reach the target accuracy of 75%, the models have not more than 72% accuracy. Maybe we could develop more models but eliminating variables that could generate noise or using different specifications to increase the accuracy.

Also, we could try to change the distribution between the test data and the training data or maybe try with some other supervised machine learning model.

