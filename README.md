# NN-scrach

## Introduction
In this project i have designed all the neural network functions from scrach and used those function to create and train a neural network for wheat seeds dataset.

## DATASET

The seeds dataset involves the prediction of species given measurements seeds from different varieties of wheat.

There are 201 records and 7 numerical input variables. It is a classification problem with 3 output classes. The scale for each numeric input value vary, so some data normalization may be required for use with algorithms that weight inputs like the backpropagation algorithm.
More information on the dataset can be found at http://archive.ics.uci.edu/ml/datasets/seeds

## Network Description

A network with 5 neurons in the hidden layer and 3 neurons in the output layer was constructed. The network was trained for 500 epochs 
with a learning rate of 0.3. These parameters were found with a little trial and error, but you may be able to do much better.
With the given description to the network. I was able to achieve an accuracy of about 91.2% on cross validation set.

For testing and prediction purposes you can create your own test set by reading the data set description from the given link.

## Prediction
for prediction purposes you can call the predict function with network weights description and i/p data as function arguments
 A sample function call looks like:
 
  predict(network, row)
  
  where network is the network description which is available as o/p after network training.
  after training use this code to get network description
  for layer in network:
	print(layer)
  
  row is the i/p data. read the dataset to create a good i/p data or find some test data for wheat seed on internet.
