## Micrograd
This is a basic implementation of the autograd package in Pytorch (``torch.autograd``). <br>
### Motivation

Neural networks (NNs) are a collection of nested functions that are executed on some input data. These functions are defined by parameters (consisting of weights and biases), which in PyTorch are stored in tensors.<br>

Training a NN happens in two steps:

**Forward Propagation** : In forward prop, the NN makes its best guess about the correct output. It runs the input data through each of its functions to make this guess. <br>
**Backward Propagation** : In backprop, the NN adjusts its parameters proportionate to the error in its guess. It does this by traversing backwards from the output, collecting the derivatives of the error with respect to the parameters of the functions (gradients), and optimizing the parameters using gradient descent.

Implementing a basic autograd engine helped me gain a better understanding of the innner workings of a neural network.
