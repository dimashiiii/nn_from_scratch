# nn_from_scratch
This project implements a basic feedforward neural network from scratch using only NumPy, without any deep learning libraries like TensorFlow or PyTorch.

FULL_CODE FILE IMPLEMENTS:
Key Components

1. DenseLayer

A fully connected layer with:

Initialization: Random weights and zero biases, with optional L1/L2 regularization.
Forward: Computes inputs @ weights + bias.
Backward: Calculates gradients for weights, biases, and inputs, including regularization.

2. ActivationReLU

Implements ReLU activation:
Forward: Outputs max(0, inputs).
Backward: Sets gradients to 0 for inputs ≤ 0.

3. Activation_Softmax_Loss_CategoricalCrossentropy

Combines Softmax activation and categorical cross-entropy loss:
Forward: Computes probabilities and loss.
Backward: Calculates gradients for backpropagation.

4. Optimizers

Optimizer_VGD: Vanilla Gradient Descent with fixed learning rate.
Optimizer_SGD: SGD with learning rate decay.
Optimizer_SGD_with_Momentum: SGD with momentum.
Optimizer_AdaGrad: Adaptive learning rate based on past gradients.
Optimizer_RMSProp: Uses moving average of squared gradients.
Optimizer_Adam: Combines momentum and RMSProp with bias correction.

5. DropLayer

Implements dropout regularization:
Forward: Randomly drops neurons based on drop_rate.
Backward: Applies the same mask to gradients.


NN_FROM_SCRATCH IMPLEMENTS:

1. Basic matrix multiplication tasks
2. Implementation of simple one neuron 
