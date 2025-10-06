
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

Our focus will be on neural networks - specifically deep neural networks (DNNs). A neural network, as the name suggests, is an arrangement of neurons placed in separate layers. Either an input/output layer or a 'hidden' layer, the number of layers is the *depth* of the network. A common way of representing the relations within a DNN is through a directed graph G = {V,E}. V being a set of neurons, E being a set of edges and   



We can represent this graphically. 

There is a sense in which a DNN is not opaque at all - after all an agent is free to inspect the shifting weights and connections of any possible network along with the actual code implementation. Our problems with opacity, which will be discussed in greater detail in Section X, concern problems with explanation. 

TA: dependence on training data ordering. 


The nature of ML algorithms make them suited for prediction rather than explanation (Shmueli 2010)


DNN