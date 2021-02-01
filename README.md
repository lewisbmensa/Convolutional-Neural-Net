# CNN from scratch

This is a README file for the Convolutional Neural Network developed from scratch.


## Conv-operator class
As an input, this takes the number of filters and the filter size. Applying this to an n x n image will return images equal to the number of filters of size (n+1 - filter size) x (n+1 - filter size)

## Max-pool class
This considers only filter size as as input. Applying this to an n x n image will return an image the size of (n/filter size) x (n/filter size)

## Softmax class
This will take as input n*n*number of filters, number of classes and returns the normalised probabilities of the class an image belongs to.

## Forward propoagation
This function takes as input an n x n and the image label and calculates the forward propogation step. This returns the output from the softmax, the cross entropy loss and evaluates the accuracy

## Training Function
Takes as input an nxn image, a label and a learning rate. This function is the back propogation step used to update all the weights of the nodes in the cnn. The return is the loss and the accuracy

## For loop
We lastly have the for loop which randomly shuffles our training data and measures the accuracy after every 100 steps. X epochs are pre determined which will cycle through all of the train data once. Lastly, the model that we have acquired from testing is evaluated on the test data and determines the accuracy of the model.
