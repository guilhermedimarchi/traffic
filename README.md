# Traffic

In order to find an acceptable accuracy it was tested changing the model configuration, like the number of layers, filters and activation functions.
Started with simple configuration having 1 convolutional layer with 16 filters 3x3, 1 pooling layer 2x2 and hidden layer with 64 neurons.
From there it was changed one variable at the time, running at least 3x times each and averaging the accuracy.
At some point this configuration best was averaging around 95% accuracy.

From there it was tested another configuration, this time with 2 convolutional layer. Repeated the same step of changing the values for the current model,
until the best average was around 98.49% with the following configuration:

- Convolutional layer 32 filters 3x3
- Max pooling 2x2
- Convolutional layer 32 filters 3x3
- Hidden layer with 256 neurons
- Dropout of 0.5 
- Sigmoid activation function
