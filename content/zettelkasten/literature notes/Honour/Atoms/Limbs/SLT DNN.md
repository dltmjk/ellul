
Sources:
[[A Falsificationist Account of Artificial Neural Networks]]
[[Computer simulations, Machine Learning and the Laplacean Demon]]


What is the use of this section: 
Brief introduction to the mechanics of DNNs 
Explain, in a commonsense way, how they work - with graphs 
Talk about how they are a class of algorithms, there are some transparent examples 


Machine learning algorithms are built on the results of statistical learning theory (SLT). SLT concerns itself with how to make accurate predictions given some empirical data. This type of relationship is modelled in the following way:

Take two spaces: an input space $X$ (Sometimes termed the 'space of instances') and the output space $Y$ (Named the 'label space'). Our task is to classify these objects into one of many, finite, categories. $X$ is the space which contains all possible objects, whereas $Y$ holds the space of all available categories (either as a real number or as a set of labels). We assume there is a predetermined class of functions, called the *hypothesis* class, in which ($h : X \rightarrow Y$). 

Each function within $\mathcal{H}$ takes a $x \in X$ and *predicts* a label $y \in Y$. A prediction rule $h$ operates by extracting or "picking up on" the relevant features of an input point $x$ and then mapping them into an output in $Y$. In this sense, $h$ is a mechanism that captures patterns or regularities in the data, so that when presented with a new, unseen input $x$, it can produce a reasonable prediction $\hat{y}$. The process of training (or learning) then consists of finding, from the hypothesis class $\mathcal{H}$, a prediction rule $h$ that best explains the relationship between $X$ and $Y$. A main assumption within SLT is that the data is governed by some unknown but fixed joint probability distribution $P(X, Y)$. 

In trying to classify these objects, we construct an algorithm which is given training examples in the format: $(x_1, y_1), (x_2, y_2)..., (x_n,y_n)$. The purpose of our algorithm is to locate a prediction rule that makes as few errors as possible. To perform this we require a learning algorithm $\mathcal{L}$ (or an optimisation procedure), for example a 'loss function', which minimises the difference between the chosen $h$ and the training dataset. 

For example, in classifying spam emails. Given an input space of emails either labelled ‘spam’ or ‘not spam’, a model should be ‘accurate’, where accuracy is defined as the probability that $(x,y)$ is a point that can be sampled on $P$. In this case, if the model is given the input (“You have won a million dollars”), which is part of the data point (“You have won a million dollars”, “spam”), it should return the corresponding $Y$ data point “spam”. 

Machine learning (ML) models are universal function approximators which, through an algorithm, implement the core logic of SLT (Hornik et al., 1989; Castro et al., 2000; Schchafer and Zimmermann, 2006). This can be done through a number of different architectures. E.g. linear models, decision trees, or neural networks. Different architectures define different ways in which the system represents and learns the underlying $h$ mapping $X \rightarrow Y$ . For example, in linear models, the architecture is simple: each input feature is multiplied by a weight and summed to produce a prediction. In comparison, decision trees split the input space into a set of decision rules in order to attain the output. Despite these differences, the logic remains static - we start with a set of training data and, through a specific procedure, approximate a certain function. 

Our focus will be on neural networks. Specifically a type of neural network dubbed a deep neural networks (DNNs). A neural network is an arrangement of neurons placed in separate layers: an input/output layer or one or more hidden layers. The number of layers is called the \textit{depth} of the network. A common way of representing the relations within a DNN is through a directed graph, where each neuron is indexed by ($i$) in layer ($t-1$) and ($j$) in layer ($t$). Each neuron ($i$) from layer ($t-1$) is connected to each neuron ($j$) in the next layer ($t$) by an edge ($e_{ij}$) for some ($t \in {1, \ldots, T}$), where ($T$) is the network's depth.

Each edge ( e_{ij} \in E ) carries an associated _weight_ ( w_{ij} ), which quantifies the strength and direction of influence between neuron ( i ) in one layer and neuron ( j ) in the next. The weights determine how the information from one layer is combined and transformed as it passes forward through the network. In addition to these weights, each neuron is associated with a _bias_ term ( b_j ), which shifts the activation threshold and enables the neuron to output non-zero values even when its weighted input sum is small or zero.

Mathematically, this operation can be expressed for a single layer as $h = \sigma(Wx + b),$ where ( x ) is the vector of activations from the previous layer, ( W ) the matrix of weights connecting the layers, ( b ) the bias vector, and ( \sigma(\cdot) ) a nonlinear _activation function_ (such as ReLU, sigmoid, or tanh). 

During training, the values of ( W ) and ( b ) are _learned_ by minimizing a chosen loss function. Typically through _gradient descent_ and its variants. This optimization process adjusts the weights in small increments opposite to the gradient of the loss with respect to each parameter (weights and biases), thereby reducing prediction error. Intuitively, learning in a DNN corresponds to progressively shaping the internal feature space defined by the weights so that the network’s output aligns with the desired target values.

Image of Gradient Descent

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

Add more to this from Sources. 

Beyond their formal structure, DNNs can be viewed as _semi-autonomous learning systems_. Once provided with data and an objective function, a DNN learns internal representations without explicit feature engineering or direct human specification of what patterns to attend to. 

The only parts a scientist has control over is the architecture and input data of the DNN. Weights are adjusted automatically. The lack of epistemic access to the method, or *decisions*, made when updating weights is one of the reasons why DNNs have been called "black-boxes" (Boge & Grunke, 2019). Other candidates for causing this black-box nature are as follows (\footnote{Examples are taken from Sogaard (2024)}): 

CITATIONS IS SOGAARD
1. Size and complexity 
	1. DNNs can have billions of parameters. Some argue that this overwhelming size makes the model "opaque" (Shrestha et al., 2021)
2. Non-linearity 
	1. A nonlinear function induces opacity due to difficulty in grasping a models "decision making" 
	2. "nonlinear structure which makes them opaque” (Joneidy & Ayadurai, 2021; Sachan et al., 2020). "
3. Lack of Grounding 
	1. DNNs are not actually connected to the world and are not derived intentionally. In particular, they "do not work in accordance with the ways humans themselves assign meaning to the reality that surrounds them” (Landgrebe & Smith, 2021, p. 2070). "
4. Semi-autonomous learning 
	1. We are not privy to the *way* and *decisions* a network makes during training. This is also called the incrementality of a system. Specifically, “learning algorithms are even more opaque because they do not rely on pre-specified instructions, but on evolving weights and networks of connections that get refined with each additional data point” (Faraj et al., 2018, §2.1),

We will -> 

ADD GRAPHS FROM SLT EXAMPLES. Overfitting and underfitting graphs 










We can represent this graphically. 

There is a sense in which a DNN is not opaque at all - after all an agent is free to inspect the shifting weights and connections of any possible network along with the actual code implementation. Our problems with opacity, which will be discussed in greater detail in Section X, concern problems with explanation. 

TA: dependence on training data ordering. 


The nature of ML algorithms make them suited for prediction rather than explanation (Shmueli 2010)


DNN