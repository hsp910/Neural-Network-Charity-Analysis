# Neural Network Investment Analysis

## Overview 

This project is being made to help decide what charities would be most succesful from the investment of a fictional company named Alphabet Soup. To do this we are given a csv filled with roughy 34,000 organizations that have recieved funding previously from Alphabet Soup. Based on this data we are given the task of determining the success of these business with future investments using tools such as neural networks for a basis. In this analysis we are using TensorFlow to create a neural network to analyze the chances of succes on each business. 

## Results

Now my results are quite abnormal and not as consistent as they should be in such an analysis. Alphabet Soup has already outlined they wish for any predictive models created by this analysis to have a roughly 75% success rate in it's testing. However as will become clear I was unable to even reach close to that goal that was laid out before me.

### Base Model

Now with the original model of this neural network I chose to only use three layers, the usual input and output layers as well as 2 hidden layers that would allow the model to in theory be better trained at it's process. The hidden layers were given a relatively small amount of neurons, 75 and 25 for the hidden layers respectively.  However, once this model was tested it was shown to only have a roughly 53.6% success rate. Deeming this far too low I set about optimizing the model through the methods I knew.

### Optimization 1: More Neurons

Simply put I increased the amount of neurons in the hidden layers to 100 and 50 in hopes that it would increase my succes rate. Then it did in fact increase the success rate of the model to 54.4%, but this is clearly still far below the goal of 75% 

### Optmization 2: Added Hidden Layer

The next step I took was to add a third hidden layer as well as adding even more neurons to it. This led to a 100-75-50 split on neurons between the two hidden layers and the output layer. Oddly enough the model became worse when this model was ran and tested with a success rate of only 49.2%. Finding this curious I pushed on in my attempts to optimize the neural network.

### Optimization 3: Changing Activations

In one final attempt to optimize the model I chose to change the activation of the first hidden layer from "relu" to "tanh" and ran the model one final time. We did increase the success rate to 53.2% which while a large gain from the last optimization, is actually still a decrease from the original optimization we did.

## Conclusion

In the end this neural network was far from capable of creating the results that Alphabet Soup was looking for in a predictive model. The final success rate gain we had was of only 54.4% which is still far below the expected 75% the company was looking for. As for reasons that this has happened I am not entirely sure. There may be issues with the way I have set up my training and testing data. Possibly my way of cleaning and changing the data provided in the csv was not the correct manner for this model. I will be looking into this in the near future and would like to edit this when I am able to provide a more sufficient answer on why this has happened.
