To illustrate this concretely, consider the classic _exclusive-or (XOR)_ problem. Suppose our network must learn the Boolean function

$\text{XOR}: {0,1}^2 \rightarrow {0,1}$

which outputs 1 for input pairs (0,1) and (1,0), and 0 otherwise. This function is not linearly separable, meaning a simple linear model cannot represent it. However, a neural network with a single hidden layer can successfully learn this mapping.

Such a network first computes a hidden representation via

$h(x; W, c) = Wx + c$

where ( W ) contains the weights connecting the input nodes to the hidden neurons, and ( c ) represents the biases. Each hidden unit then passes its output through a non-linearity function which yields 

$h_i = \max{0, (Wx + c)_i}.$

Finally, the output layer combines these hidden activations through another weighted sum,

$f(x; W, c, w, b) = w \cdot \max{0, h} + b.$

Here, the distribution of _weights_ across layers enables the network to transform the input space into one where the XOR outputs become linearly separable. 