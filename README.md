# Project-7-Multi-Layer-Perceptron-2




# MLP layers:
Multilayer perceptron is the same as building dense layer of the neural network. 
According to the problem solution we have create three custom models and we 
are doing exactly that. 

# Model1:
Type: sequential () #keras

Layer1:

Activation: relu

Number of neurons:50

Input size: same as shape of the data

Layer2:

Activation: relu

Number of neurons:25

Layer3:

Activation: sigmoid

Number of neurons:1

Optimizer: Adam

Metrics: accuracy


# Model2:

Type: sequential() #keras

Layer1:

Activation: relu

Number of neurons:100

Input size: same as shape of the data

Layer2:

Activation: relu

Number of neurons:75

Layer3: Dropout

Activation: relu

Number of neurons:25

Layer4:

Activation: sigmoid

Number of neurons:1

Optimizer: Adam

Learning rate: 0.01

Metrics: accuracy

# Model3:

Type: sequential () #keras

Layer1:

Activation: LeakyReLU

Number of neurons:50

Layer2:

Activation: LeakyReLU

Number of neurons:25

Layer3:

Activation: sigmoid

Number of neurons: 1

Optimizer: RMSprop

Metrics: accuracy

ARCHITECTURE OF 3 MLP MODELS (COMMON FOR BOTH
Task 1 AND Task 2):

MODEL 1:

There are three dense layers with 50, 25 and 1 neuron at the end with 
activation as relu, relu and sigmoid (linear for task1).

MODEL 2:

In this model we have 4 layers, with 100,75,25 and 1 as the number of neurons 
and here I added the dropout layer between the 2nd and 3
rd layer. And I have 
used relu, relu, relu and sigmoid (linear for task1) activation function.

MODEL 3:

In this model, I have used three layers, the number of neurons is 50, 25, 1 and 
the optimizer, I have used is RMSprop and the activation function on the final 
layer is sigmoid (linear for task1) as it is doing the task of classification.
Comparison of the 3 MLP models:

Below are the three accuracies for the three models, I have seen that the 
Model 3 is more accurate compared to the model 1 ad 2 but it does not matter 
that much when we look at the accuracies. But here we have to see the false 
negatives, because in this case false negatives should be less. And yes, the least 
number of false negatives are in the model 3 and the greatest number of false 
negatives are in the model 2.

Model1: Accuracy: 0.9950041631973355

Model2: Accuracy: 0.9908409658617818

Model3: Accuracy: 0.9966694421315571

AS, I have mentioned in the previous answer int the p
art 1, we have to follow some rules to achieve good a
ccuracy but again that is not the convection, i.e. mo
st of the times you don’t follow that and still get b
etter accuracy.

I have used the same models as I have used above but 
there is a slight change and that is the models are h
aving binary cross entropy as loss function and the s
igmoid as the activation function in the final layer 
as we are doing the task of classification.

# Comparison of the 3 MLP models with the Normal SVM, Random Forest and Decision Tree classifier:

Here we note that the random forest and decision tree classifier performed
better than the three MLP models, but here there is a catch I got same 
accuracy for random forest and decision tree classifier but the main difference
in the classification of number of False positive and false negatives. It depends 
on what we are looking for, If we want to classify the anomaly as bad and we 
want to make sure that all the anomaly be detected even with some 
compromise the we might accept the latter case (false positive is more)
Why did random forest and decision tree outperform other models?
The decision tree divides the items by lines and it does not define how distant 
is the point from the lines, this acts as an advantage for the decision trees and 
The MLP model also performed well, I think with good picking for better 
structure of the models the accuracy could have been increased also.













