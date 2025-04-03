What I need to answer 

1. I need to start with how these black box algorithms are being used in the real world. They are already being employed, how are people justifying their trust in these things. 
	1. Perhaps historical examples of previous scientific instruments, could be useful. The microscope comes to mind. 

Examples
1. Alphafold (DURMLJ pg 1) 
	1. Create atomic notes for these later 
2. BenevolentAI (DURMLJ pg 1)

Connection between [[Process Reliabilism]] AND CR
- Duran article on connecting the two 
	- Which article is this? 
- Why are we using process reliabilism? Why is this the best way to tackle this problem 

Why do we need to seek justification
> The first interpretation addresses how algorithms involve multiple complex elements (functions, variables, decisions, data, etc.) in their specification, coding, execution, and maintenance. This means that little can usually be said about how these algorithms cluster data, which criteria are used for creating categories, and overall why algorithms behave the way they do. This interpretation is captured in the epithet ‘black-box’ algorithms as a way to express how far removed algorithms sometimes are from human insight. The second interpretation sets the focus on our limited capacities to say something meaningful about the output of an algorithm [51, 649]. That is, no human being (or group of human beings) can know which functions, variables, decisions, data, etc. are relevant to a given output. - DURMLJ

how CR leads to justification or trust

What is epistemic opacity and how does it lead into all of this
1. We need to answer why algorithms behave the way they do 

how are black box algorithms different from humans e.g. a doctor just making a prediction, or other scientific instruments
1. How do we justify the results of scientific instruments? 
	1. The algorithms merits cannot be determined by association with a body of scientific knowledge
		1. By adequacy to empirical data or diverse theoretical constructs (DURMLJ)
	2. If opaque stuff is just another scientific instrument, shouldn't we use it results holistically? 
		1. or are we only speaking about the cases where opaque stuff is the only tool at disposal. 
2. What is justification in relation to the output of a scientific instrument. 

why aren't ML algorithms explainable just off backpropogation and other stuff

why can't you trust the ML model but not a doctor

## General Structure
1. Give examples of algorithms that are already being used
	1. Alphafold, find others
	2. Maybe talk about how scientists justify their internal mechanisms. Perhaps try to find older variants of the algorithms and compare them. 
	3. What is the difference between a scientific process/instrument and a human (e.g. a doctor)
	4. How do we trust algorithms\other opinions already?
		1. We a human performs any sort of algebra, they are not acquainted with every single natural number (Ground for Trust) 
		2. Therefore, how do we perform calculations 
			1. Certain methods confer reliability (How to tie this in with process reliabilism)
				1. For example, mathematical induction
					1. But how are these methods valid? 
				2. Why do these methods confer reliability? 
2. Why are opaque machine learning algorithms different from other algorithms. Why are they different from other scientific instruments, why are they different from people? 
	1. Normal scientific instruments 
		1. You can detect artifacts and give explanations 

# Questions I need to answer
1. What motivates this as an interesting philosophical question
	1. Examples
		1. Climate Prediction Models
		2. Disease classification
			1. Alphafold, LIME (Transparent), BenevolentAI
		3. Self driving cars
		4. Criminal justice 
	2. Try to find an example that is new but also had a predecessor that was more explainable. 
2. What is a black box algorithm 
3. How are these black box algorithms different from:
	1. Other algorithms
		1. There are no internal models or representations 
			1. Why doesn't backpropagation count?
		2. There is no way to implement interventions ('what if we do X') or counterfactuals ('What if we do Y instead of X')
			1. While they can establish certain connections between input and output data (for example, medicine and patient reaction)
				1. They cannot implement certain counterfactuals, like modifying the medicine slightly and seeing the result. They cannot analyze past decisions with questions of if different treatment regiments were used. 
					1. Can doctors do this? 
		3. This class of problems is called the interpretability problem of AI systems. 
	2. Other scientific instruments 
	3. Human beings 
4. How is epistemic opacity related to all of this? 
	1. Computer systems are **epistemically opaque** but not **epistemically inaccessible**
		1. Research David Armstrong Eliatic principle 
			1. This seems like overkill. Maybe rename inaccessible into something else
		2. We have access to the code, the training rules implemented and the machinery the system runs on. We also have access to its [runtime operations](https://www.science.org/content/article/how-ai-detectives-are-cracking-open-black-box-deep-learning) 
		3. The same ML architecture can lead to different results
			1. For example, Hebbian plasticity (Neurons that fire together wire together) makes the algorithm *plastic*. 
				1. This means that given two ML algorithms with exactly the same input data and training rules. They will diverge in their results. Upon analysis different neuron blocks will fire in the two models despite an identical input.  
	2. Why can't we just explain ML algorithms off backpropagation and other stuff?

## Things to keep in mind
1. How can I motivate every jump 
2. Usage of AI $\rightarrow$ Black box problems $\rightarrow$ Difference between different algorithms $\rightarrow$ Why we use PR $\rightarrow$ Jump from PR to CR

## Things I should probably talk about 
1. Interpretability
2. Surveyability
3. Transparency
4. Robustness


