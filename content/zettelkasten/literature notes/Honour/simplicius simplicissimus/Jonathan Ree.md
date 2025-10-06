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

Section 1: 
1. SLT Rundown
2. DNN Rundown
	1. Training and Deployment usage 
3. Opaqueness Brief Introduction 
4. Why transparency is important 
	1. Doctor and example [[Conceptual challenges for interpretable machine learning]]
	2. Skogaard example in hOutline 

Section 2: 
We argue for a distinction between two types of scientific instruments: x and y. This is a division similar to those drawn by philosophers of science in the past (Baird, Harre, Heidelberg)

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
	3. As Deude points out (Find other source). When certain instruments encompass both categorises their nature of justification 
		1. Therefore, for ML we can break the instrument into two parts. 
			1. Training acts as the way the DNN picks up on a certain phenomenon 
			2. Deployment is how the DNN actually models this phenomenon 
		2. Both stages are liable to justification and opacity provides problems for both. 
2. How do we justify the reliability of *causal instruments*
3. How do we justify the reliability of *model instruments*

NTV 
1. Ortmann Conditions for trust in an instrument 
	1. Koskinen advances two important conditions here. First, there needs to exist some- one with an understanding of the instrument in question. Second, this someone needs to be a moral agent who can assume responsibility for the epistemically relevant and value-laden decisions they have taken. - Relevant quote pg. 6/80
2. This has the advantage over trusting instruments because you can hold these agents accountable if the instrument falters. 


Section 3: Models 
1. What are models? 
	1. Literature definitions 
	2. In some ways DNNs are models in a strict sense. One could argue that the actual neural network weights and biases (and to a lesser extent the actual computation behind these calculations) are the sense in which DNNs are models. However, it would be unfair to say this is what we are interested in. Instead, what we are interested in is what is encoded by the DNN, as a representation, when making its prediction. These are the models which concern us. 
2. What is an explanation 
	1. I shall argue that what Jack and Dr. Jill seek is a causal account of why f made the particular prediction it did. Following the interventionist tradition, I regard an explanation as causal insomuch as it identifies a set of variables which, when set to certain values, are sufficient to bring about the outcome in question [[Conceptual challenges for interpretable machine learning]]
3. At what point do we cease being able to give explanations? 
	1. Property of opacity as rendering the lack of explanations to an agent. 


How does ExAI work? 
1. What is the goal of ExAI
	1. To answer questions of the type: 
		1. Why did model f predict outcome ˆyi as opposed to alternative y′i =/= yi for input vector xi 
2. ML models fail to represent their targets in a way that makes them similar to their targets. However, as a model instrument, you can demarcate certain parts of the model (e.g. as in cogsci modelling) to see the causal relationships between different parts of the model allowing for some understanding (Bujisman) 
3. Using similar models to arrive at a common concept and seeing how this is phenomenon directed 
	1. "To understand the specifics of RA for ML, we start by considering RA for analytical models as a contrast class. Here, the basic methodology (often called ’triangulation’) goes as follows (Weisberg, 2006): First, identify a group of sufficiently diverse models that all predict a common result.Footnote 3 Second, investigate whether all these models share a robust property, such as the reliance on a specific variable or a generalising theoretical property that can be proven. Third, provide interpretations of how the robust mathematical strands in a model capture the causal structure of a given empirical phenomenon of interest" [[Beyond generalization; a theory of robustness in machine learning]]
4. 




Intro: 
Reverse order - > DNNs are black boxes -> so they do not produce explanation 


At what point do we cease being able to give explanations.  TA: What properties induce opaqueness - Tim Raz ML Interpretability: Simple isn't easy - for examples 

ML models fail to represent their targets in a way that makes them similar to their targets. However, as a model instrument, you can demarcate certain parts of the model (e.g. as in cogsci modelling) to see the causal relationships between different parts of the model allowing for some understanding (Bujisman) 

If DNNs do not represent their targets - they are just result producing instruments and cannot be reliably held towards producing explanations because the nature of explanations in instruments is very specific and requires causality 