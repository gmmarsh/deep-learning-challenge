# deep-learning-challenge

Overview of the analysis: The purpose of this analysis is to develop a binary classification model that will assist Alphabet Soup with selecting applicants for funding that will have the best chance of success in their ventures. The model will predict if the venture will be successful or not sucessful. 

Data Preprocessing

What variable(s) are the target(s) for your model?

"IS_SUCCESSFUL" column

What variable(s) are the features for your model?

APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested

What variable(s) should be removed from the input data because they are neither targets nor features?

EIN and NAME—Identification columns


Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

The first model in the Starter_Code.ipynb consisted of an input layer, two hidden layers and an output layer. The first hidden layer contained 80 neurons and the relu activation function. The second layer contained 30 neurons and the relu activation function. The output layer contained one neuron and the sigmoid activation function.

The relu activation function was used for both hidden layers because it handles complex non-linear data patterns well.

The sigmoid activation function was used for the output layer because the model was trained to make a binary classification of successful or not successful.

The quantity of neurons for each hidden layer was chosen based on the guidance from the starter code.

Were you able to achieve the target model performance? Yes, the optimization model was able to produce a test accuracy of 0.7289 which is slightly higher than the test accuracy of the starter code model of  0.7287.

What steps did you take in your attempts to increase model performance?

In the first layer, the number of neurons changed from 80 to 128. In the second layer, the number of neurons increased from 30 to 64.

An additional hidden layer was also added with 32 neurons and a relu activation function.

A dropout of .5 was also added to each layer to help reduce overfitting.

Summary:

The base model found in the Starter_Code.ipynb file produced a test accuracy of 0.7287.

The optimization model found in the Optimization.ipynb file produced a test accuracy of 0.7289

My recommendation is to move forward with the process of entering the optimization model into production.

Other binary classification models could be considered as well such random forest classifier and logistic regression.