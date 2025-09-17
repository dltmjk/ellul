Section 1: Trust in regards to scientific instruments 
1. How do we normally go about trusting scientific instruments 
	1. There needs to be an agent involved 

Section 2: DNNs as a scientific model/instrument 
1. The DNN is a scientific instrument 
2. How does it differ from other scientific instruments.

Section 3: What are the methods we can use to trust DNNs.  
1. ExAI
	1. This differs from the type of explanation we are after. Scientific explanations are different from ExAI which seek to just explain internal mechanisms
	2. Can this be redeemed in any way? 

Difference Between DNN and Scientific Instruments
1. DNNs approximate a function
2. What function do they approximate exactly? 
	1. [[Functional Concept Proxies and the Actually Smart Hans Problem - What’s Special About Deep Neural Networks in Science]]
	2. They develop functional proxies for concepts, which is why they are able to generalise so well in scientific research. Because sometimes these functional proxies are things humans are not aware of. They specialise from non obvious features. 
		1. The problem with this is that they are vulnerable to attacks

Ways DNNs are different from other scientific models/instruments 
1. What did I already write 
	1. [[Two Dimensions of Opacity and the Deep Learning Predicament]]
		1. DL models are instrumental in a way that is different from other scientific models 
		2. ExAI isn't helpful
2. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]]
	1.  Sullivan (2022b, p. 128) argues that it is not the opacity of an ML model that potentially hinders understanding, but rather the ‘link uncertainty’ attached to it, that is, “the amount, kind, and quality of scientific and empirical evidence supporting the link connecting the model to the target-phenomenon
	2. "As a main example, Sullivan discusses Schelling’s model of segregation: Here, it seems irrelevant how the model is implemented for it to promote understanding of segregation phenomena in cities; all that matters is that we know how to connect its in- and outputs to evidence about people’s housing behavior."
	3. Scientists may gain "objectual understanding" from the outputs of a DNN system
		1. "As Räz and Beisbart (2022, p. 12) argue, scientists might gain objectual under standing directly from the use of ML models like AlphaFold2, where objectual understanding concerns a subject matter or phenomenon on the whole, as in ‘S understands P’; P being the relevant topic, subject matter, or phenomenon,6 Thus, scientists might understand ‘the protein universe’ better, directly from AlphaFold2’s outputs. But this contrasts with understanding why proteins fold the way they do, where ‘understanding why’ is usually taken to be intimately connected to explanations."
			1. Similar to other scientific instruments. For example, a microscope engenders objectual understanding. 
			2. However - "Stated differently, even though AlphaFold2 has increased our understanding of protein folds, it hasn’t rendered protein folding any more understandable, by virtue of falling short of providing a mechanism—something that could explain why proteins fold the way they do. Hence, even if some things may be understood more or less directly with the help of models like AlphaFold2, it remains fair to say that the amount of understanding that transpires from opaque ML models is in general rather limited, and to some extent even ‘off-target’."
	4. Therefore, we need to understand how the model relates to a particular target. 

What is the problem? 
1. Given this black box-nature, how can DNNs truly help us advance science? For, in the words of Raghu and Schmidt 
	"Many standard applications of deep learning [...] focus on prediction—learn- ing to output specific target values given an input. Scientific applications, on the other hand, are often focused on understanding—identifying underlying mechanisms giving rise to observed patterns in the data." pg.44 [[Two Dimensions of Opacity and the Deep Learning Predicament]]
2. Implications of opacity to science 
	1. 


Definition of Opacity 
1. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]]
	1. "If we take ML models to be opaque in the sense that it is difficult to understand why their outcomes arise (Beisbart, 2021, p. 11643)"
	2. [[Humphrey's Epistemic Opacity]]
2. [[Degrees of Epistemic Opacity]]
	1. Paper aim is to get a better understanding of what epistemic opacity is. 
		1. From Humphrey's ([2009]([[Extending ourselves Computational science, empiricism, and scientific method]])) original definition - Referred to as 'weak epistemic opacity'
		2. Epistemic opacity as coming in degrees. If we can demarcate degrees, we can go from higher to lower degrees of epistemic opacity. 
			1. How is this done? - Expert knowledge. Scientific knowledge helps to "move around" opacity. Not to remove it completely. 
			2. "we can claim confidently that scientific practice is tightly related to the notion of epistemic opacity, and further that it has an impact on how epistemic opacity is to be understood."
3. [[On the Opacity of Deep Neural Networks]]/[[Deep Learning Opacity in Scientific Discovery]]
	1. Susceptibility to Training Data Ordering
		1. The model is volatile given a specific training history. The ordering of training data affects the resulting model.
	2. Inability to understand what parts of the model perform which functions.
		1. If we created a DNN which mimics the function of a certain traditional classifier model, we would be unable to match the parts of the DNN that are analogous to the traditional model.
	3. Inability to meaningfully understand or explain the process behind a certain output
		1. When we examine a DNN we are unable to find out which function or algorithm it implemented in order to classify data because it was constructed autonomously during the training-phase.

Ways of Dealing with Opacity 
1. ExAI
	1. Methods for explanation in ExAI
		1. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]] pg.2 
	2. "Scientists’ interest in what is usually called ‘eXplainable AI’ (XAI) should be rather high accordingly. But under one reading at least, “‘explanation’ here refers to an understanding of how a model works, as opposed to an explanation of how the world works” (Rudin, 2019, p. 206). Hence, even if XAI succeeds, can we really expect an understanding of “underlying mechanisms” or “how the world works” from it?" pg. 44 [[Two Dimensions of Opacity and the Deep Learning Predicament]]

Problems With ExAI
1. ExAI Inputs needs to be made testable -> Feeds into pragmatic treatment of AI Tools. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]]
	1. However, the methods of explanation in ExAI are different from explanatory theories in philosophy of science. 
	2. "Indeed, several critical voices (Buijsman, 2022; Krishnan, 2020; Páez, 2019) have urged that the term ‘explanation’ in XAI is largely misguided: The ouputs of XAI methods are nothing like the claims or propositions involved in explanations in the sense familiar to philosophers."
	3. Structure 
		1. Why is explanation useful? 
			1. Historical examples of explanation vs mere remedy - Scurvy and British sailors 

Why Reliability? 
1. While we may not know how an ML system works, we know what makes it work better than other ML systems. When put into domain specific contexts, we allow for experts to make adjustments that make these systems more *reliable*. Therefore, we should be focusing on the ways we can increase this reliability. 
