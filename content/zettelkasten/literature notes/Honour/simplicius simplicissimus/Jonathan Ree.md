Intro: [[Intro;Problem]]
Section 1: [[SLT DNN]]
Section 2: [[Instruments]]
Section 3: [[Models]]

Papers: 
Find ExAI and explanation paper 
Go through each paper in tabs. Highlight each ones use - e.g Raz is good for what properties induce opaqueness - and build an essay plan around the best ones. 
Look at Boge 2 Dimensions after plan has been written. 


Intro: 
1. Examples
2. DNN as being labelled black boxes
	1. Why? 
3. This prevents them from giving explanations 
4. Why is transparency important?
	1. Doctor and example [[Conceptual challenges for interpretable machine learning]]
		1. Skogaard example in hOutline 
		2. Especially given that these tools are being used for medical diagnosis, medical testing and other high-stakes contexts. 


Section 1: 
1. SLT Rundown
2. DNN Rundown
	1. Training and Deployment usage 
	2. Add part about how a DNN is self learning and autonomous 
		1. For the first property, which prevents transparency of the processes, we take up the term semi-autonomy (Boge & Grunke, 2019) [[The Automated Laplacean Demon; How ML Challenges Our Views on Prediction and Explanation]]
3. Opaqueness Brief Introduction 
4. Add something about the Training Process of DNNs and more about autonomous-learning 


Section 2: 
We argue for a distinction between two types of scientific instruments: x and y. This is a division similar to those drawn by philosophers of science in the past (Baird, Harre, Heidelberg). It's common to label DNNs as 'models', but the ways and contexts of which these models are used has not been explored fully. 

1. [[Instrument vs Experiment ]]
	1. How they are used in the context of scientific discovery (Deude)
		1. ML Pipeline 
			1. [[Beyond generalization; a theory of robustness in machine learning]]
			2. Along with Deude 
		2. Used to produce results in the process of discovery. 
		3. There a number of reasons for accepting the classification of instrument given their place within a larger process of discovery. Given that statistical algorithms also are classified into similar categories. They are not experiments because they provide results not claims in need of justification 
	2. Whether they pick up or model certain phenomenon 
		1. However, certain problems have been raised, in the analogous study of computer simulations, of whether these tools are experiments, instruments, inferences, or problem solving techniques. The tension comes down to whether these tools "pick up" on phenomena and respond in a certain manner or if they model a certain phenomena. 
			1. They are causally related as they pick up on a phenomena and then come to model it. 
		2. Furthermore, if DNNs are modelling instruments, how they they model these representations. They themselves aren't models, but instead hold models to make predictions? 
			1. DNNs present a new epistemic challenge as their modelling/representation capabilities arise naturally in response to input. They naturally catch on and model a phenomenon
		3. This is the way to resolve the *causal* vs *model* dilemma. Just combine them, say that the challenge is with how they can fit into both categories. 
		4. The way that each instrument is justified depends on the type of instrument they are. 
	3. As Deude points out (Find other source). When certain instruments encompass both categories their nature of justification need to include the way that their relationship with both categories are mediated
		1. Therefore, for ML we can break the instrument into two parts. 
			1. Training acts as the way the DNN picks up on a certain phenomenon 
			2. Deployment is how the DNN actually models this phenomenon 
		2. Both stages are liable to justification and opacity provides problems for both. 
	4. One one hand a DNN will always pick up on a function (over-fitting or adversarial examples) - > this is causal in nature. However, we need to make sure it picks up on the correct function. 
	5. In this case, there is another division. 
		1. During the *causal instrument*, we are explaining our justification for the construction of this instrument -> that is was constructed in a way that means it will work. We defer to expert knowledge in these cases and their techniques 
			1. Why doesn't the justification of the training stage mean that it has guaranteed the reliability of the deployment stage? 
				1. Adversarial examples. 
		2. However, for the *model instruments* we need to justify that the model is indeed accurate. 
2. Justification for both requires testimony
	1. [[Analysis of Beliefs Acquired from a Conversational AI]]

TA: If trust requires transparency, how do we justify trust in *causal* and *model* instruments. 

[[NTV Opacity]]
1. Ortmann Conditions for trust in an instrument 
	1. Koskinen advances two important conditions here. First, there needs to exist some- one with an understanding of the instrument in question. Second, this someone needs to be a moral agent who can assume responsibility for the epistemically relevant and value-laden decisions they have taken. - Relevant quote pg. 6/80
2. This has the advantage over trusting instruments because you can hold these agents accountable if the instrument falters. 
3. Therefore, there needs to be an ability for an agent to give reasons for the functioning of an instrument. In order words they need to be able to 
	1. Conversely, the epistemic transparency of a model is understood as its ‘analytic tractability’, defined as an epistemic agent’s ‘ability to decompose the process between model inputs and outputs into modular steps, each of which is methodologically acceptable both individually and in combination with the others
	2. In other words - Humphreys opacity 
4. This means that they have to be able to give "reasons" or explanations for their instruments 
	1. What exactly is reason giving? What form does it take in the philosophy of science. 

Redo Explanations section - Start again and plan thoroughly. 
[[Explanations]]
What is an explanation?
	1. In relation to computer science - is abstracting 
		1. Find the source with the american scientist article - cosmology? 
	2. Literature 
		1. Appealing to correlations is not an accurate way of producing explanation. Instead, there needs to be a line of causation [[The Automated Laplacean Demon; How ML Challenges Our Views on Prediction and Explanation]]
		2. Prediction and explanation in regards to the scientific instrument 
	3. I shall argue that what Jack and Dr. Jill seek is a causal account of why f made the particular prediction it did. Following the interventionist tradition, I regard an explanation as causal insomuch as it identifies a set of variables which, when set to certain values, are sufficient to bring about the outcome in question [[Conceptual challenges for interpretable machine learning]]
	4. Explanation refers to concepts which are agent-directed. 
		1. [[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]
	5. Explanation then requires the identification of concepts and the discovery of the causal way they are related. 
6. Explanations take a certain form when we apply them to models 
7. Is the training stage of DNNs really opaque? 
	1. At what point do explanations fail to give a reason? 

[[Explanations, Opacity, Models]]

Opacity - At what point do we fail to be able to give explanations for DNNs? 
1. Raz ML Interpretability: Simple isn't easy
	1. Go through multiple models and how we give explanations for the functioning, making them non-opaque. 
2. Run this all together with "what a model is" and how we normally explain these models and how they explain the underlying phenomena. 
	1. How explanation arises out of certain things we are able to do to the model 
	2. [[Conceptual challenges for interpretable machine learning]]
		1. How does this relate with simpler statistical techniques? 
3. DNNs failing to semantically decompose their targets



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
		2. "An example given by her (280 ff.) is the imagined ability of dog D to treat anotherdog, M, at times as a hunting partner, at times as a threat. This behavior of D towardsM might still be different from D’s behavior towards yet another dog, N , who wasalways treated as a threat by D. It hence seems plausible that D has distinct conceptsof M and N , as well as distinct concepts hunting partner and threat. Crucially,the things to be combined are representations of particulars and their ways of being,and the latter representations can be combined in different ways with the former ones" [[Functional Concept Proxies and the Actually Smart Hans Problem - What’s Special About Deep Neural Networks in Science]]
			1. Carnap and Concepts 
		3. [[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]
	3. However, can we represent these concepts in a way that lends itself to explanation? 
6. How can models provide explanation 
	1. "Herbert Simon distinguished between “basic science” and “applied science” (Simon, 2001), a distinction sim- ilar to explaining versus predicting. According to Si- mon, basic science is aimed at knowing (“to describe the world”) and understanding (“to provide explana- tions of these phenomena”). In contrast, in applied sci- ence, “Laws connecting sets of variables allow infer- ences or predictions to be made from known values of some of the variables to unknown values of other vari- ables.”" [[To Explain or to Predict?]]
	2. Difference between models made to explain and to predict 
7. Idealised models - add something about this 
8. However, prediction models can still be used for explanation 
	1. Through causal graphs or something? 


Explanations and Opacity
1. We know what explanations are in regards to models
2. Different types of models 
	1. [[DARPA’s Explainable Artificial Intelligence Program]] for graph 

A model of the world that is liable to semantic explanation is very different from how a neural network may choose to encode this information. 
DNN's encode models, but not in a way that is semantically decomposable - e.g. liable to explanation. (Deude, Sullivan) - Wittgenstein quote. 

How does ExAI work? 
1. What is the goal of ExAI
	1. To answer questions of the type: 
		1. Why did model f predict outcome ˆyi as opposed to alternative y′i =/= yi for input vector xi 
2. ML models fail to represent their targets in a way that makes them similar to their targets. However, as a model instrument, you can demarcate certain parts of the model (e.g. as in cogsci modelling) to see the causal relationships between different parts of the model allowing for some understanding (Bujisman) 
3. Using similar models to arrive at a common concept and seeing how this is phenomenon directed 
	1. "To understand the specifics of RA for ML, we start by considering RA for analytical models as a contrast class. Here, the basic methodology (often called ’triangulation’) goes as follows (Weisberg, 2006): First, identify a group of sufficiently diverse models that all predict a common result.Footnote 3 Second, investigate whether all these models share a robust property, such as the reliance on a specific variable or a generalising theoretical property that can be proven. Third, provide interpretations of how the robust mathematical strands in a model capture the causal structure of a given empirical phenomenon of interest" [[Beyond generalization; a theory of robustness in machine learning]]

Why ExAI fails in determining reliability 
1. ExAI methods are numerous, but they revolve around two main techniques: feature attributions and model inspection. Model inspection, follows from research in neuroscience and records which neurons fire at which inputs in attempt to categorise them.  
2. Arguments for the explanatory nature of the model can only be used to illuminate the underlying model, not as an argument for the reliability of the model. [[Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead]]

For explanations 
1. ExAI can be a possible method, it situates DNNs within a larger context of scientific discovery and other methods have to be implemented in order to make these results explainable 

For reliability 
1. We should not use ExAI methods to justify the functioning of certain DNNs. Instead we should opt towards algorithms that are interpretable by nature. 




Intro: 
Reverse order - > DNNs are black boxes -> so they do not produce explanation 


At what point do we cease being able to give explanations.  TA: What properties induce opaqueness - Tim Raz ML Interpretability: Simple isn't easy - for examples 

ML models fail to represent their targets in a way that makes them similar to their targets. However, as a model instrument, you can demarcate certain parts of the model (e.g. as in cogsci modelling) to see the causal relationships between different parts of the model allowing for some understanding (Bujisman) 

If DNNs do not represent their targets - they are just result producing instruments and cannot be reliably held towards producing explanations because the nature of explanations in instruments is very specific and requires causality 