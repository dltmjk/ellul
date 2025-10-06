Intro: [[Intro;Problem]]
Section 1: [[SLT DNN]]
Section 2: [[Instruments]]
Section 3: [[Models]]

Section 1 covers the internal workings of a DNN while clarifying how exactly they are being used within scientific contexts. 

Section 2 goes over the classification of DNNs within categories present within the philosophy of science. 

Explanation in regards to scientific instruments 

Section 3: Models and opacity. Models cannot represent their targets, therefore failing to meet the criterion of justification 

Section 4: Explanation and usage 

This paper makes the following novel contributions to the discussion on DNN (ML) usage within science. 

Reliability is in large part determined by giving explanations for functioning of a system in a way that is intelligible. 

"For an instrument to be reliable is for the output of its detection process to cap-ture the targeted features of the phenomenon and thus permit accurate measure-ments that represent those features. But since we have no direct access to thephenomenon outside of some detection device, there is no way to directly comparethe phenomenon with the instrumental response. Instead, instrumental reliability issupported by the stability of instrumental results in different places and times usingthe same experimental protocols (replicability) and stability of results among verydifferent kinds of experiments (reproducibility or convergence). For NMR to reli-ably indicate the atomic structure of a protein is for the signals detected (chemicalshift) and measured (decay curves) to reflect the distance and rotational anglesbetween atoms present in the molecules constituting the protein." Sandra NMR spectroscopy 

**Go back to scientific instrument section and continue from there** 

Structure 
1. Introduction 
	1. Alphafold example 
		1. The problem was with the lack of explanation - Use Boge quote, find and keep. 
	2. Other examples - for prediction vs understanding
		1. [[Prediction versus understanding in computationally enhanced neuroscience]]
	3. Problem [[Intro;Problem]]
	    1. DNNs are “black boxes”, or epistemically opaque which, as some researchers have suggested, presents a uniquely problematic epistemic situation.
	    2. Cover a small toy example of how these models are 'opaque'
	4. Quick recap of surrounding literature
	    1. The problem is that we are treating the DNN as an epistemic source in itself, instead of an instrument within the context of a larger process of scientific discovery
	5. Thesis: 
		1. This thesis is an investigation into what exactly a DNN is, how exactly it functions (is it an experiment or model) in relation to other scientific models (representational status) and how it fits into scientific discovery. Answering all of these questions helps us in deciding how researchers are expected to utilise and treat these tools.
	6. We seek to establish the DNN as a model. As a model we conclude two things:
		1. The lack of explanatory power from DNNs is because of its lack of being grounded in a theory 
		2. DNNs do not contain 
2. [[SLT DNN]]
	1. Formalisation

===Rework this into something else===
[[Instrument vs Experiment]] 
	1. Experiments establish causal phenomena whereas instruments just take advantage of them 
	2. Experiments have different epistemic expectations. 
	3. Instruments only explain things, and have their results valid, in the presence of a larger theory. 

In answering what they are, we can understand what norms should surround their usage. We argue that a large part of misunderstanding comes about from DNN

What type of instrument
	1. Causal or model instrument 
		1. Are they a causal instrument? 
			1. They are not, because if we appeal to a simple neural network/transparent neural network-> really this is building a function through a mathematical method. It cannot be a causal instrument because there is a potential to pick up on a different function than intended, whereas a causal instrument will pick up on the same one. 
			2. Their training allows them to build up to a function which is a model of the world 
		2. Therefore, they are a model
			1. How do we normally justify the results of a model 
			2. Through explanation. Justification is usually given through testimony by an agent who understands the inner workings. This is the case with scientific trust. 
Rework Experiment vs Instrument discussion into causal vs model instrument discussion. 

Causal 
1. Technically the model picks up on certain phenomena and reacts accordingly. - "phenomena" being the data set that is fed into the computer to produce a pattern or a prediction. 
	1. However, due to adversarial attacks, it fails to do this consistently. It depends heavily on the ordering of the training data 
2. Therefore, DNNs are models



What is a model exactly? 
The way we justify the reliability of models is by close analysis of its internal logic. In this case, the theory of machine learning (the weights and biases). Why does this fail? Why can't we just appeal to this? 

How do models work, how to guarantee their reliability 

The explanatory nature of models depend in large part to their transparency. Because DNNs are unable to fulfil this, what exactly are they? 

This fails because...



Opacity 
1. Types of opacity, how they interfere with giving reasons for workings of a model 
2. Go over how reliability has been framed uptil this point - not in terms of reason giving 
3. The main type of opacity for DNNs is providing reasons that demarcate certain parts of the model. Generating a causal graph for the model. 

Opacity as the prevention for abstraction. 


Transparency
1. Overview of transparent vs explainable models 
	1. Transparent being - designed with representation in mind
	2. Explanation being - techniques to account for opacity 
		1. Fails because Zerelli 2019, Deude Models 

DNNs, working as models when applied in a certain context. 
"Basically linear model of a visual neuron’s receptive field yields the qualitative expectation, prior to any calculation, that an increase in the amount of light falling in the excitatory field of the neuron, will result in an increase in the model’s predicted response" [[Prediction versus understanding in computationally enhanced neuroscience]]

A neural network, when employed in its original context as modelling the perceptual field holds great explanatory power. The sub-parts of the model are directly analogous with the target phenomenon (neurons in a frog). Counterfactual's are easily implemented and causal relationships can be determined. 

[[To Explain or to Predict?]]



Wittgenstein quote 

Primer for next section: 
However, if scientists had access to the internal concepts a model picks up on when producing it outputs. Wouldn't this, if grounded in a specific experimental context, allow for a greater objectual understanding of the phenomena at hand? 

(DNNs could provide explanation if only in a very causal manner. Seeing how the model arranges certain variables and how these variables effect each other - counterfactuals. These things when grounded within a certain theoretical or experimental context would allow for a greater objectual understanding)

However, this fails because DNNs do not contain semantic representations in a causal manner. 
Need to argue against DNNs storing causal explanations? Bujisman. 


What are scientific models? [[TA;Models]]
	1. What are the epistemic responsibilities of a model? 
		1. Do they need to provide explanation - no, explanation is provided 
		2. How is explanation provided in scientific models? 
			1. Problems with explanation hinge on how we treat the role of DNNs within scientific experimentation
	2. How are they reliable 
		1. We have good reasons that they are analogous to the target phenomena and represent it. 
			1. These things are not opaque because we can construct higher level reasons that act as explanations for their behaviour. 
			2. The things that cloud the construction of these reasons are things that induce opaqueness. 
		2. How are models analogous? 
			1. What is the mechanism that makes them analogous? 
		3. Technical Opaqueness overview 
			1. Different ways opaqueness has been characterised:
				1. Like what opaqueness meant a system. We are saying that it stops the forming of explanations. Humphreys may have felt that it makes a system un-surveyable. 
				2. Opaqueness is a property applied to a system that stop an agent from constructing explanations for its reliability 
					1. Main opaqueness is that we are unable to find what parts of the system do what. This is the problem with representation. 
		4. We justify the use of model instruments based on the fact that they are analogous to their target phenomena. However, DNNs are not really analogous - they cannot be because they do not encode a semantic representation of its target. 
			1. Representation in this way is similar to neuroscience - termed functional representation. 
				1. They encode things relationally, but not in a way that lends itself to human explanation. 
			2. Problem with transparency 
				1. They argue that DNNs encode things in a far too simplistic manner, which will pose problems later down the line if these explanations are speciously applied to justify reliability as well
					1. Matthew L Leavitt and Ari Morcos. Towards falsifiable interpretability research.
					2. Cynthia Rudin. Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead
			3. Model opacity is really a problem of representation. We need to be given reasons in a way that is easily and semantically understandable. The functioning of our own brain is not dissimilar to the structure of a DNN. However, explanation in cognitive science requires a degree of abstract representation (e.g. this part of the brain does X).
		5. DNNs do not have this -> they cannot have this, what are the other ways we can justify their use? 


What have we established 
1. DNNs are *model instruments* and do not require explanatory potential without a guiding theory 
2. Despite being *model instruments* they do not acquire justification in the same way other model instruments do, because it is impossible to justify any representation. 
3. Therefore, we need to find alternate ways of justifying their results 

AI needs to be part of a wider process of discovery (Duede)

Certain pragmatic uses of AI use:
What does our presentation of DNNs mean for how they CAN be used within scientific discovery 
Causal models can be created in view of a theory, these can be used for explanation. Only if there is a method of interpretation (Bujisman)


However, DNNs will continue to be used in scientific experimentation. How do we ensure reliability and justify their results? 

Therefore, if DNNs are *model instruments* but cannot be justified in a way similar to other model instruments. 

Our conclusion - DNNs need to be built and used in a pragmatic way, as part of a wider process and stop treating DNN claims as full justifications but only as results. 



Thesis: ML algorithms are accused of producing prediction without explanation. However, this confusion is because these algorithms are assumed to be experiments instead of instruments. An experiment explains something about the underlying mechanism, whereas an instrument only produces results.

Therefore, our only concern with DNNs isn’t whether they can explain the underlying mechanism, neither do ExAI methods which hope to explain the DNN functioning matter. What matters is whether this DNN is reliable.

IF THE DNN DOES NOT ENCODE A SEMANTIC REPRESENTATION OF ITS TARGET -> THEN WE CANNOT APPEAL TO TRANSPARENCY EXPLANATIONS WHEN ANALYSING ITS RELIABILITY. IT MUST BE DONE IN OTHER WAYS. 








What is a DNN?



Conclusion of this section:  
DNNs do not produce explanation along with their output, as previously conceived. They are perfectly valid acting as simple scientific instruments which generate outputs, along as there is an agent (scientist) who can take responsibility.

NTV/Social Epistemology/Testimony Section

Normal ways in which scientific instruments are opaque

DNN opacity in specifics.

Chapter 7 of Simulating Science book is immensely useful.

Opacity is always agent specific. There is nothing that makes something opaque generally, it is always towards an agent. DNN opacity arises out of the intermixed complexity and scale of their systems. However, it is perfectly possible to produce a transparent rendition of a simple DNN system. Showing that opacity is not guaranteed.

Argue against Humphrey’s idea of essential epistemic opacity.
Does ExAI remedy this? / Provide explanation for opacity.

Things to cover
DNNs are instruments and not experiments, and therefore are not epistemically responsible for producing explanation alongside their outputs.
Therefore, as an instrument, we need to focus on the reliability of a given tool. Does transparency help in producing reliable machine learning algorithms?
Problems with ExAI as just letting us understand how input gets to output but doesn’t necessarily help with increasing reliability
DNN usage needs to be situated in the context of a larger process of scientific discovery.