# Pruning Neural Networks using Tensorflow

I implement two types of pruning techniques on the MNIST dataset:

1. Weight Pruning - make individual weights equal to 0 - remove connections between neurons
2. Unit Pruning - Making entire columns of the weight matrix equal to 0 - remove a neuron completely

The code is structured as follows:

**1. DataLoader** - This class loads the data and creates training and testing sets<br />
**2. NeuralNetworkPruner** - This class implements the main network. It initializes the architecture and has different methods for fitting on the data, pruning it and predicting on a test dataset

How to use the code: Use the **fit_prune()** method to fit your model on the data. It will fit the model and then prune it using the specified pruning technique. Finally, use **predict()** method to generate predictions on unknown dataset.
