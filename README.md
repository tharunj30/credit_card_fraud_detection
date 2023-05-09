# Credit-card-fraud-detection
CREDIT CARD FRAUD DETECTION USING NEURAL NETWORKS(ANN)

About dataset:

The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.


Proposed solution:
Artificial neural networks with different number hidden layer using keras making it more deeper for training model to train it .
In the first MLP, neural network with single hidden layer without drop and with drop.
 Neural network with two hidden layers in the second MLP and  neural network with three hidden layers in the third MLP.
 In the first MLP, there are three layers in the network: an input layer, a hidden layer, and an output layer.
The input layer has 29 neurons, the hidden layer has 65 neurons, and the output layer has one neuron.
 A defined custom activation function was utilised, one without dropout and the sigmoid function was used in the output layer
It was subsequently determined that our model was overfitting the data set and that dropout was necessary.
In the second model, there are four layers in the network: an input layer, two hidden layer, and an output layer.
The input layer has 29 neurons, the two hidden layer has 65 neurons each, and the output layer has one neuron.
For one of the hidden layers, a special activation function(custom) was used, while ReLU was used for the other.
The sigmoid function was used in the output layer.
However we had already determined that our model would overfit the data set without the use of dropout, So we continued using dropout.
In the third model, there are five layers in the network: an input layer, three hidden layer, and an output layer.
The input layer has 29 neurons, the three hidden layer has 65 neurons each, and the output layer has one neuron.
For one of the hidden layers, a special activation function was used, while ReLU was used for the other two.
The sigmoid function was used in the output layer with the dropout.


 

