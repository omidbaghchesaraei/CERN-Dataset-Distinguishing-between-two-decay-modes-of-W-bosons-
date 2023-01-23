# CERN-Dataset-Distinguishing-between-two-decay-modes-of-W-bosons-
The CERN Dataset: I created a neural network model using TensorFlow that can distinguish between two modes of W boson decay with an accuracy of 94%.

The W boson is a fundamental particle. Together with the Z boson, it is responsible for the weak force, one of four fundamental forces that govern the behavior of matter in our universe.

My research is based on two modes of W bosons (Wmunu & Wenu) as follows:

1) Wmunu: An event was selected if there was one (and only one) global muon in the event.
2) Wenu: An event was selected if there was one electron in the event.

I use two datasets, which are available on the CERN Open Data portal, Wmunu.csv and Wenu.csv, each of which contains 100,000 records.

The first thing I do is train a simple Neural Network (two hidden layers, each with 64 neurons and an activation function of sigmoid, epochs = 500), and then plot accuracy and loss graphs on the training and validation datasets to find a balance between the model that is underfitting and one that is overfitting(or converging), resulting in a model with a good fit.

By the 500th epoch, validation loss is decreasing, which indicates that the model is underfitting. However, after the 500th epoch, validation loss is converging. At the 500th epoch, when the model is either perfectly fitted or in a local minimum, the neural network model achieved an accuracy of 94%.
