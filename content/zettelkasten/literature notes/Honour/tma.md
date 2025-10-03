Structure 
1. Introduction 
	1. Alphafold example 
		1. The problem was with the lack of explanation - Use Boge quote, find and keep. 
	2. Problem
	    1. DNNs are “black boxes”, or epistemically opaque which, as some researchers have suggested, presents a uniquely problematic epistemic situation.
	3. Quick recap of surrounding literature
	    1. The problem is that we are treating the DNN as an epistemic source in itself, instead of an instrument within the context of a larger process of scientific discovery
	4. Thesis: 
		1. This thesis is an investigation into what exactly a DNN is, how exactly it functions (is it an experiment or model) in relation to other scientific models (representational status) and how it fits into scientific discovery. Answering all of these questions helps us in deciding how researchers are expected to utilise and treat these tools.
2. What is a DNN?
	1. Formalisation
3. [[Instrument vs Experiment]] 
	1. Experiments establish causal phenomena whereas instruments just take advantage of them 
	2. Experiments have different epistemic expectations. 
	3. Instruments only explain things, and have their results valid, in the presence of a larger theory. 
4. What type of instrument
	1. Causal or model instrument 
		1. Are they a causal instrument? 
			1. They are not, because if we appeal to a simple neural network/transparent neural network-> really this is building a function through a mathematical method. It cannot be a causal instrument because there is a potential to pick up on a different function than intended, whereas a causal instrument will pick up on the same one. 
			2. Their training allows them to build up to a function which is a model of the world 
		2. Therefore, they are a model
			1. How do we normally justify the results of a model 
			2. Through explanation. Justification is usually given through testimony by an agent who understands the inner workings. This is the case with scientific trust. 
5. What are scientific models? 
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
				1. They argue that DNNs encode things in a far too simplistic manner, which will pose problems later down the line if these explanations are speciously applied to justify reliability aswell
					1. Matthew L Leavitt and Ari Morcos. Towards falsifiable interpretability research.
					2. Cynthia Rudin. Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead
			3. Model opacity is really a problem of representation. We need to be given reasons in a way that is easily and semantically understandable. The functioning of our own brain is not dissimilar to the structure of a DNN. However, explanation in cognitive science requires a degree of abstract representation (e.g. this part of the brain does X).
		5. DNNs do not have this -> they cannot have this, what are the other ways we can justify their use? 
6. Therefore, the usage of DNNs should be done in a way that an expert can give reasons (e.g. trained with good i.i.d etc...) for why the potential for it to become unreliable did not arise.
	1. Justification is based around different factors, such as it was trained with a dataset that does not seem non-adversarial, or the loss is quite low and it responds correctly to different training examples. 


Thesis: ML algorithms are accused of producing prediction without explanation. However, this confusion is because these algorithms are assumed to be experiments instead of instruments. An experiment explains something about the underlying mechanism, whereas an instrument only produces results.

Therefore, our only concern with DNNs isn’t whether they can explain the underlying mechanism, neither do ExAI methods which hope to explain the DNN functioning matter. What matters is whether this DNN is reliable.

IF THE DNN DOES NOT ENCODE A SEMANTIC REPRESENTATION OF ITS TARGET -> THEN WE CANNOT APPEAL TO TRANSPARENCY EXPLANATIONS WHEN ANALYSING ITS RELIABILITY. IT MUST BE DONE IN OTHER WAYS. 






What is a DNN?

Cover a bit of the opacity problem. While these concerns will be raised briefly here, they will be covered in detail later on.

Instruments vs Experiments – What exactly are DNNs?

What is an instrument

What is an experiment

In answering what they are, we can understand what norms should surround their usage. We argue that a large part of misunderstanding comes about from DNN

How do they fit into scientific taxonomy and how do they differ?

Scientific Instruments

Causal vs Model instruments

What is a model

Are DNNs like other scientific models? Are they like mathematical models?

Do models normally have an explanatory quality?

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