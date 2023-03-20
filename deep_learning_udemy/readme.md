# Deep Learning A-Z 2023 - Udemy

## ANN Intuition

ANN: Artificial Neural Networks

Important points:
- The Neuron
- The Activation Function: is the process applied to data within the neuron. Explore commonly used activation functions, and trade offs.
- Practical Application
- How Neural Networks Learn: gradient descent; stochastic gradient descent; backpropagation

Imitates what has been observed in the human brain.

Synapse: Term used when data is exchanged between the dendrites and the axon. This term is used when referring to the passing of signals in our neural networks.

The neuron receives a list of input values, and has one output value. These inputs are independent variables. You can determine what variables will enter your neural networks.

You must either standardize the values of your independent variables or normalize them. These processes keep your variables within a similar range so it is easier for you NN to process them. (Also necessary to avoid bias)

Output values can be continous, binary or categorical.

It is important to remember so you can keep things clear in your mind when working through this; both the inputs on the left and the outputs on the right are single observations.

The weight is assigned to each synapse for the signal that passes along it. Weights are how NN learn. Based on each weight, the NN decides what information is important, and what isn't. The weight determines which signals get passed along or not, or to what extent a signal gets passed along. The weights are what you will adjust through the process of learning.

The neuron takes all the weights it has received and adds them all up. It then applies an activation function that has already been applied to either the neuron itself, or an entire layer of neurons. This function facilitates whether a signal gets passed on or not. That signal goes on to the next neuron down the line then the next, so on and so forth.

Activation functions:
- The Threshold Function: Binary output; step function
- The Sigmoid Function: Better suited to probabilities when applied at the output layer of your NN.
- The Rectifier Function
- Hyperbolic Tangent Function