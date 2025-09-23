Detailed Outline
___
Introduction
1. Alphafold example 
2. General prevalence of DNNs 
3. What has already been researched + How is this research different from other research. 
4. Structure of the essay 

## GO THROUGH hOUTLINE and TABS to construct essay plan

[[Scientific Instruments]]
1. Trust in instruments 
	1. What exactly is trust? Can we trust an object
		1. Trust requires an agent. When we trust someone not to rob us, we are trusting in their moral conscience. We do not trust objects, we rely on them. Agents can be held responsible if they breach our trust, objects cannot. When we say we “trust” an objects, we mean that it is a reliable object - one that functions according to our expectations. (HOutline)
2. Breakdown of Instruments 
	1. Instruments assist in knowledge production during research. 
	2. *instruments that interact with the world* & *instruments that model the world*
		1. This distinction arose in the 17th century "the trend-setting differentiation between “mathematical” and “philosophical” instruments emerged (see for example Shapin 2006, Benett 2011, Warner 1990 and 1994, van Helden 1983 and 1994)." (Kletzl/Neges Dis. pg.108)
		2. The line between both is blurred 
			1. "First, as has been pointed out by many scholars, this distinc- tion primarily mirrored a newly-emerging social boundary, but it does not have much to do with underlying epistemic principles. The same functions of instruments, like the possibility to perform different kinds of measurements, could be regarded as part of a philosophical as well as of a mathematical instrument, dependent on who used the instrument and in what context (see van Helden 1983, 65)."
			2. In our later discussion of DNNs we will find that certain uses of DNNs could fit into either category 
			3. Why is this spiel still important? 
					1. The types of ways these two instrument types are reliable differ. 
	3. We can justify the OUTPUT of instruments if they are reliable. 
		1. How do these two instruments differ in their reliability 
			1. Consistently exploiting causal pathway vs acting analogously to the world 
3. What is the function of instruments? 
	1. Another example that is worked out in much detail is Michael Heidelberger’s discussion of four different roles that instruments can play in experimental setups (see Heidelberger 2003, 146ff). (Kletzl Diss pg. 109)
		1. Producing phenomena (Microscopes, telescopes, air pumps)
			1. Also splitting up phenomena into small parts (e.g. spectrometer)
		2. Making phenomena behave in certain ways 
			1. E.g. making phenomena "pure"
		3. Imitative function 
			1. Produce effects that appear in nature but on a smaller scale 
		4. Representative role 
4. Definition of opaqueness 
	1. Humphreys Definition 
		1. Here a process is epistemically opaque relative to a cognitive agent X at time t just in case X does not know at t all of the epistemically relevant elements of the process. A process is essentially epistemically opaque to X if and only if it is impossible, given the nature of X, for X to know all of the epistemically relevant elements of the process (HOutline)
		2. Burrel expands 
			1. They are opaque in the sense that if one is a recipient of the output of the algorithm (the classification decision), rarely does one have any concrete sense of how or why a particular classification has been arrived at from inputs. Additionally, the inputs themselves may be entirely unknown or known only partially.”
		3. What does explain mean? 
		4. What is an epistemically relevant element? 
			1. An element which is known to an agent and can be used by them to explain other elements within the system or the systems output.
	2. Why are certain instruments opaque towards an agent
		1. Technical opaqueness
			1. Non-understanding of each moving part. 
		2. Social opaqueness 
			1. Barriers to double checking. 
	3. Therefore, we need to move into NTV 
		1. Social epistemology literature 
5. Conclusion
	1. With all this established. Why exactly do DNNs pose a problem? 
		1. Summarise main argument of next section. 
6. To Add Somewhere: 
	1. Explanatory use of instruments within science. Instrument allows us to study the causal effect we are exploiting. 

[[What's so special?]]
1. Common argument that DNN is a black box. 
	1. Why exactly is a DNN a black box? What fuels these common notions. 
2. What type of instrument is a DNN 
	1. Is it an *instrument that interacts with the world* or a *instrument that models*
		1. It's a bit of both depending on it's use. 
		2. Example of *instrument that interacts with the world*
			1. Could the training data be the discovery of functions of causal relationships with the world? or is this something that is kept exclusively for *instruments that model*
		3. Example of *instrument that models*
			1. Most statistical methods 
3. Ways in which DNNs are unreliable 
	1. Transparency arguments 
		1. [[Knowledge and The Trustworthiness of Instruments]] pg.162

How do we ensure reliability? 
1. Through ExAI? 
	1. Problems with ExAI
	2. It doesn't fulfil the common explanations we refer to in the philosophy of science. 
2. Alternate methods 
	1. Only reliability within pragmatist notions of ML. 

Outline
___
Section 1: Trust in regards to scientific instruments 
1. How do we normally go about trusting scientific instruments 
	1. There needs to be an agent involved 
2. Agency in regards to scientific instruments 
	1. Necessary Trust View 

Section 2: DNNs as a scientific model/instrument 
1. The DNN is a scientific instrument/How does it differ from a normal scientific instrument
	1. How does the DNN pose problems to our traditional conceptions of scientific trust. 
	2. Opacity, Explain opacity in regards to normal scientific instruments 
	3. How are DNNs qualitatively different? 

Section 3: What are the methods we can use to trust DNNs.  
1. ExAI
	1. This differs from the type of explanation we are after. Scientific explanations are different from ExAI which seek to just explain internal mechanisms
	2. Can this be redeemed in any way? 


Notes
___
Why is a DNN a scientific instrument 
1. [[Scientific Instruments]]
	1. Define what a scientific instrument is. Go into slight detail between the differences between scientific instruments 
	2. Give example

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
3. Examples of opacity in science 
	1. [[Thing Knowledge]] pg.3 
	2. Faradys device. No-one denies that it works, just how it worked. Even today, people are unsure. 


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
		2. [[Instruments, Agents, and Artificial Intelligence]]
			1. 'Local approaches' allow us to understand how a model changes in regards to a particular input 
			2. However, this doesn't yield global understanding. 
	2. Inability to understand what parts of the model perform which functions.
		1. If we created a DNN which mimics the function of a certain traditional classifier model, we would be unable to match the parts of the DNN that are analogous to the traditional model.
	3. Inability to meaningfully understand or explain the process behind a certain output
		1. When we examine a DNN we are unable to find out which function or algorithm it implemented in order to classify data because it was constructed autonomously during the training-phase.

Problems With Humphrey's Opacity 
1. [[Thing Knowledge]] pg.13
	1. Nobody understands completely how their telephone works. We should not seek understanding at the level of individual belief. 
	2. Therefore, we should switch to a view in which we consider social epistemology of science. 

Ways of Dealing with Opacity 
1. ExAI
	1. Methods for explanation in ExAI
		1. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]] pg.2 
	2. "Scientists’ interest in what is usually called ‘eXplainable AI’ (XAI) should be rather high accordingly. But under one reading at least, “‘explanation’ here refers to an understanding of how a model works, as opposed to an explanation of how the world works” (Rudin, 2019, p. 206). Hence, even if XAI succeeds, can we really expect an understanding of “underlying mechanisms” or “how the world works” from it?" pg. 44 [[Two Dimensions of Opacity and the Deep Learning Predicament]]
2. Why can't we just justify models with more training data to see if it's predicting the correct function? - Because we don't know?

Problems With ExAI
1. ExAI Inputs needs to be made testable -> Feeds into pragmatic treatment of AI Tools. [[Put it to the Test Getting Serious About Explanation in Explainable Artificial Intelligence]]
	1. However, the methods of explanation in ExAI are different from explanatory theories in philosophy of science. 
	2. "Indeed, several critical voices (Buijsman, 2022; Krishnan, 2020; Páez, 2019) have urged that the term ‘explanation’ in XAI is largely misguided: The ouputs of XAI methods are nothing like the claims or propositions involved in explanations in the sense familiar to philosophers."
	3. Structure 
		1. Why is explanation useful? 
			1. Historical examples of explanation vs mere remedy - Scurvy and British sailors 

Why Reliability? 
1. While we may not know how an ML system works, we know what makes it work better than other ML systems. When put into domain specific contexts, we allow for experts to make adjustments that make these systems more *reliable*. Therefore, we should be focusing on the ways we can increase this reliability. 
