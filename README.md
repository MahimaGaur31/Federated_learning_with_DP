# Federated_learning_with_DP



Federated Learning simulation using pysyft and Duet for image classification on healthcare data.
DP-SGD implementation modeled after techniques presented within Deep Learning with Differential Privacy and A General Approach to Adding Differential Privacy to Iterative Training Procedures.
Run multiple models with different Gaussian noise differential privacy to determine  privacy and accuracy the trade-off.
Understanding the trade-off between differential privacy and accuracy of the models.


#Architecture:

#Central Server
Contains the aggregated model.
Sets connections with edge devices and receives the gradients based on the training data edge devices contain

#5 Edge devices
Contain the training data (images and corresponding labels)
Once the connection is established, they send the pointers to data to the Central server and compute the gradient updates
The gradient updates are sent upstream to the central server which updates the weights of the model
