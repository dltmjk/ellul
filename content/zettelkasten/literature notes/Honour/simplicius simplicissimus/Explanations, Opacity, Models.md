TA: Where do DNNs actually keep concepts? What is a model in a DNN? 

What is an explanation?
	1. In relation to computer science - is abstracting 
		1. Find the source with the american scientist article - cosmology? [[Explanations]]
	2. Literature 
		1. Appealing to correlations is not an accurate way of producing explanation. Instead, there needs to be a line of causation [[The Automated Laplacean Demon; How ML Challenges Our Views on Prediction and Explanation]]
		2. Prediction and explanation in regards to the scientific instrument 
	3. I shall argue that what Jack and Dr. Jill seek is a causal account of why f made the particular prediction it did. Following the interventionist tradition, I regard an explanation as causal insomuch as it identifies a set of variables which, when set to certain values, are sufficient to bring about the outcome in question [[Conceptual challenges for interpretable machine learning]]


First Past The Post:
To recap: we have argued that the training process of a DNN must be justified as a causal instrument. Whereas the DNN in deployment must be justified as a model instrument. 

In this section we will argue that the common arguments for opacity present no real problems for justifying the result for the training of a DNN. If they are simply instruments which produce a DNN, then they have to be justified in a similar way another causal instrument would be under expert reliability 

[[T-DNN]]

Why doesn't the normal justification of -> this has picked up the best function work for DNNs? Because we are interested in the decisions made that are understandable towards a human agent. Especially in high stakes decision making 

How do we justify the results of a causal instrument. This is done in reference to its reliability. How are causal instruments reliable -> if they are constructed in a manner that prevents faulty operation. Whereas model instruments require other criterion of justification. 

As a causal instrument, we require the same architecture to produce the same output every time the same data is put in. As other author argue, we do not need to be privy to the way that the DNN organises this information, as justification arises out of expert decision rules during the construction of training. 

Models however need to be explainable in order for the results to be justified. Furthermore, in making a model explainable, we can also explain the underlying phenomena. Bujisman


How do model instruments work? 
Model instruments are a class of things, either material or formal in type, that represent a certain target phenomena through approximation, idealising the phenomena, or simplifying it. 

Section 3: Models 
1. What are models? 
	1. Literature definitions 
		1. "Bewilderingly diverse sets of models coexist and enjoy continued success across scientific disciplines that are at different degrees of maturity. This set includes single equations (e.g., the Ising model [26] in quantum physics), physical scale models that are copies of the phenomenon" [[Deep Neural Networks as Scientific Models]]
		2. According to Ludwig Boltzmann’s first modern definition of of models, a model is ‘a tangible representation [. . . ] of an object’ [[Models, Algorithms, and the Subjects of Transparency]]
2. Types of Models
	1. Explanatory, descriptive, predictive 
		1. [[To Explain or to Predict?]]
3. How do models actually work for other instruments. I.e. how are they phenomenon targeted 
	1. C-Schema stuff
	2. Isomorphic relation 
		1. [[Analogue Models and Universal Machines. Paradigms of Epistemic Transparency in Artificial Intelligence]]
4. These are representations 
	1. What is required of the representation? 
		1. "its essential directionality and its capacity to allow surrogate reasoning and inference" [[An Inferential Conception of Scientific Representation]]
5. DNNs are models, but in what sense? 
	1. Discrepancy between actual architecture and encoded models 
		1. In some ways DNNs are models in a strict sense. One could argue that the actual neural network weights and biases (and to a lesser extent the actual computation behind these calculations) are the sense in which DNNs are models. However, it would be unfair to say this is what we are interested in. Instead, what we are interested in is what is encoded by the DNN, as a representation, when making its prediction. These are the models which concern us. 
	2. How do their representations function? do they acquire concepts
		1. Yes they do acquire concepts, we have good reasons for believing that this is the case. 
		2. "An example given by her (280 ff.) is the imagined ability of dog D to treat another dog, M, at times as a hunting partner, at times as a threat. This behavior of D towardsM might still be different from D’s behavior towards yet another dog, N , who wasalways treated as a threat by D. It hence seems plausible that D has distinct conceptsof M and N , as well as distinct concepts hunting partner and threat. Crucially,the things to be combined are representations of particulars and their ways of being,and the latter representations can be combined in different ways with the former ones" [[Functional Concept Proxies and the Actually Smart Hans Problem - What’s Special About Deep Neural Networks in Science]]
			1. Carnap and Concepts 
		3. [[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]
	3. However, can we represent these concepts in a way that lends itself to explanation? 
6. How can models provide explanation 
	1. "Herbert Simon distinguished between “basic science” and “applied science” (Simon, 2001), a distinction sim- ilar to explaining versus predicting. According to Si- mon, basic science is aimed at knowing (“to describe the world”) and understanding (“to provide explana- tions of these phenomena”). In contrast, in applied sci- ence, “Laws connecting sets of variables allow infer- ences or predictions to be made from known values of some of the variables to unknown values of other vari- ables.”" [[To Explain or to Predict?]]
	2. Difference between models made to explain and to predict 
7. Idealised models - add something about this 
8. However, prediction models can still be used for explanation 
	1. Through causal graphs or something? 

3. Explanation refers to concepts which are agent-directed. 
		1. [[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]
	5. Explanation then requires the identification of concepts and the discovery of the causal way they are related. 

This raises the question, do DNNs encode concepts? 

Before answering this, we must see how models normally encode concepts. 

Do DNNs encode concepts in a causal way? 

1. Explanations take a certain form when we apply them to models 
2. Is the training stage of DNNs really opaque? 
	1. At what point do explanations fail to give a reason? 

Opacity - At what point do we fail to be able to give explanations for DNNs? 
1. Raz ML Interpretability: Simple isn't easy
	1. Go through multiple models and how we give explanations for the functioning, making them non-opaque. 
2. Run this all together with "what a model is" and how we normally explain these models and how they explain the underlying phenomena. 
	1. How explanation arises out of certain things we are able to do to the model 
	2. [[Conceptual challenges for interpretable machine learning]]
		1. How does this relate with simpler statistical techniques? 
3. DNNs failing to semantically decompose their targets





Explanations and Opacity
1. We know what explanations are in regards to models
2. Different types of models 
	1. [[DARPA’s Explainable Artificial Intelligence Program]] for graph 

A model of the world that is liable to semantic explanation is very different from how a neural network may choose to encode this information. 
DNN's encode models, but not in a way that is semantically decomposable - e.g. liable to explanation. (Deude, Sullivan) - Wittgenstein quote. 



Explanations 
1. What is an explanation in the philosophy of science? 
2. Correlation is not an explanation. There needs to be a causal mechanism 
	1.  [[The Automated Laplacean Demon; How ML Challenges Our Views on Prediction and Explanation]]
3. When these tools are used, what is needed is a causal explanation especially for models 
4. If we return to model instruments, how do we normally explain them
	1. Historical example? 
	2. Models need to be justified in a very particular way within the philosophy of science 


Overview of how models are justified 
1. To establish: 
	1. Models are phenomenon targeted and conceptually understandable 
		1. Boge explanation document 
		2. Add a graph or something 
	2. Phenomenon oriented 
		1. Source:
	3. Conceptually understandable 
		1. Source:
2. Types of models - look at other planning doc 
	1. [[To Explain or to Predict?]]
	2. Explanatory, descriptive, predictive 
3. Formalisation of models 
4. How are DNNs models 




5. Explanations, therefore require concepts
6. Do DNNs have concepts? 
	1. Concept literature - find including deude 
7. Explanation requires the discovery of these concepts and finding out how they are linked within the modelling of the DNN 

[[Isomorphic Models]]


Models
1. What are models? 

Opacity
1. How is explanation giving done in relation to simpler models 
	1. TA: Mills method of difference 
2. There is a way to point to a certain part of the model and say - this is what it does and be sure. 


Models