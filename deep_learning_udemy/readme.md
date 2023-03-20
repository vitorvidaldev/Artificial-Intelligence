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

You can implement a hidden layer that sits between the input and output layers. Not all synapses are weighted. They will either have a zero value or non zero value.

You have the single row of input variables on the left. The arrows that represent weighted synapses go into the large neuron in the middle. And on the right, you have the output avlue. This is called a Single-Layer Feedforward Neural Network. The output value above is represented as Y. This is the actual value. We are going to replace taht with ^Y, which represents the output value. The difference between Y and ^Y is at the core of this entire process. In order for our network to learn we need to compare the output value with the actual value. Then we will apply a cost function, which is one half of the squared difference between the output value and actual value. This is just one commonly used cost function, there are many.

The cost function tells us the error in our prediction. Our aim is to minimize the cost function. The lower the cost function, the closer ^Y is to Y, and hence, the closer our output value to our actual value.

A lower cost function means higher accuracy for our network. Once we have our cost function, a recycling process begins. We feed the resuling data back through the entire NN. The weighted synapses connecting the input variables to the neuron are the only thing we have any control over.

We need to repeat this until we scrub the cost function down to as small a number as possible, as close to zero as it will go.

We feed the variables through the weighted synapses and the neuron to calculate our output value, ^Y. Then the cost function is applied and the data goes in reverse through the NN.

Remember, the input variables do not change. It is only the weight of the synapses that alters the cost function comes into play.