# A comprehensive investigation on CIFAR10 Deep Neural Network(Tensorflow-keras)
This code implements a deep neural network for the CIFAR10 dataset, with the goal of achieving high accuracy and low loss.

In the next step, the SELU activation function has been selected for the hidden layers, and the weights have been initialized for self-normalization. The accuracy and loss of the model have been plotted for the train and validation data without changing the number of neurons and layers.

To investigate the effect of BatchNormalization, the SELU activation function has been changed, and BatchNormalization has been added after each layer except the last one. The results have been compared to the previous step.

Next, transfer learning has been used to predict whether there is a horse or not in each photo. Using 6000 data from the dataset, the best model from the previous step has been frozen, and the necessary changes to the last layer have been made for prediction in the new problem. The accuracy and training duration have been reported, and then all the layers have been unfrozen, and the accuracy and training duration have been compared to the previous state.

To evaluate the performance of different optimizers, SGD, SGD with momentum, Nesterov SGD with momentum, AdaGrad, Adam and Nadam with constant learning rate have been tested on the model. The accuracy and loss obtained after 50 epochs for all optimizers have been plotted in a graph.

Finally, the model has been regularized using dropout, MCdropout, and l1-l2 methods, and the resulting accuracy and loss have been plotted for 100 epochs. These regularization techniques have been applied to prevent overfitting and improve the generalization of the model.

In summary, this code presents a comprehensive approach for the CIFAR10 dataset that includes experimenting with different network architectures and training techniques. The various steps and methods used in this implementation can be useful for other image classification tasks as well.
