TO DO: 

**Start section with the common platitude of DNNs being black boxes. Use a quote (like sullivans) of the link uncertainty. Argue that more attention needs to be paid to where exactly opacity is introduced.**


[[Analogue Models and Universal Machines. Paradigms of Epistemic Transparency in Artificial Intelligence]]
Useful source for finding out what epistemically opaque element -> and other things mean. 
[[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]
Very good source. -> Explain ability as being subjective and dependant on the stakeholder. DNNs as hoping to pick up on a concept/function. 

What is a concept? How do DNNs pick up on it? 

[[Sources of Opacity in Computer Systems; Towards a Comprehensive Taxonomy]]
pg. 3 graphs. Continue from discussion on NTV how these are socio-technical sources of opacity, which are remedied by the existence of an agent who can take responsibility. The opacity which affects DNNs are more technical in nature. 

Furthermore, does opacity refer to the system itself? or the behaviour of the system towards a human agent? Good source: [[Models, Algorithms, and the Subjects of Transparency]] - Also a very good way to structure your introduction (The problem: The argument:).

"While a consensual and unified definition of epistemic opacity in AI is missing in the literature, the earliest and most frequently cited definition is the one proposed by Humphreys" - Good, rewrite. 

Opacity is always in reference to a human agent, which manifests out of certain properties in a system. - pg. 3. DNNs can “can approximate virtually any function of interest to any desired degree of accuracy, provided sufficiently many hidden units are available” (Hornik et al., 1989). 

Relation to theory-dependence: How does a DNN differ from other statistical algorithms -> because it doesn't have theory [[The Automated Laplacean Demon; How ML Challenges Our Views on Prediction and Explanation]]

Alphafold Diss - What does it mean for a result to be scientific knowledge? Does scientific knowledge require explanation? 

To sort out: The specific role of explanation within knowledge 
Where does explanation come into normal scientific instruments 





Does the model need to accurately represent the underlying mechanism in order to be trustworthy? 
Potentially very useful source: [[Model Evaluation An Adequacy-for-Purpose View]]

It seems like the immense success of DNNs within non-scientific contexts have unconsciously fostered the idea that it more than an algorithm. For example, 
"AlphaGo’s defeat of Lee Sedol in 2016 is another celebrated example of DL in interactive reinforcement learning contexts. Similarly, better than human deep reinforcement learning successes were achieved by OpenAI in Dota2 competitions, and CMU’s Libratus and Plaribus poker algorithms. More recently, tasks in modern natural language processing (NLP) have also seen ostensible breakthroughs by becoming competitive with human performance."  [[Machine understanding and deep learning representation]]

In losing sight of the actual structure and use of a DNN, we have forced upon it a role that it is not required to serve. 

To answer: why is it a problem that DNNs predict without explanation? Usually we can see the way a machine got from input to output - This serves as explanation. At which point is opacity introduced? 

Why isn't the justification that "oh it goes to gradient descent enough? "



To Write: The advantage that treating DNNs as scientific instruments gives us. We treat the DNN as one part of the scientific process. We only have problems with opaqueness when we treat a DNN as standing in for all parts of the scientific process. However, 

1. Note down each reason for opacity 
2. Reasons for opacity 
	1. Evaluate as a scientific instrument 

We should only care about reliability, if the DNN is a scientific instrument. Can reliability ever be secured? 

Source for not trusting objects, only relying - C. Thi Nguyen (Koskinen pg. 7)

Arguments for Opacity. 

There is a property $\chi$ that when applied to a scientific model makes it opaque. The lack, or toning down, of this property increases the *transparency* of a system. If more than two $\chi$ properties are present, the lowering of one doesn't change the opaqueness of a system. If we imagine a system that is opaque because of its dimensionality, modifying the size should not make a difference to the overall opaqueness. In attempting to find which properties actually guarantee opaqueness, we can look at examples of inherently transparent statistical algorithms, of which both decision trees and naive bayes classifiers are examples. 

Decision trees are generally considered to be fully transparent algorithms (Mittelstadt et al., 2018, Skogaard pg. 227). They function as a nonlinear flowchart structure made up of nodes.

![[Pasted image 20250926193228.png]]
MAKE OWN IMAGE

A decision tree progresses through these nodes depending on the content of some input data. For example, a decision tree constructed in order to diagnose a fever may return “yes” if given a temperature of “40.5C” and “no” if given a temperature of “37C”. All decision trees are theoretically computable by hand. A large enough tree, with millions of parameters, could be worked through given enough time.

For example, size is commonly thought of as a candidate for opaqueness.


In what qualities does a DNN differ from these two algorithms? 


Zerelli “Tractability/Intelligibility/Fathomability Distinction” 

Categories for Opaqueness 
Fathomability 
Intelligibility 
Tractability 

Zerilli argues for model opacity along the lines of _linearity_ and _dimensionality_. A linear system with fewer dimensions is more _fathomable_ than an alternate higher dimensional system. In which _fathomability_ concerns a human observer who, in the former low-dimensional case, is able to “contemplate the entire model at once” (Lipton 2017, 4) (Zerelli, 7). Therefore, dimensionality and fathomability are inversely correlated. An unfathomable system, for example, would be an extremely large computer simulation model with billions of parts. However, as long as this simulation maintains linearity, it retains another two of Zerelli’s properties - intelligibility and tractability. Tractability is whether a model can be run on a machine whereas intelligibility is if the relationship between a model’s subparts can be determined, despite size.

Zerelli’s speaks of opacity in respect to these properties. For example, a computer program which multiplies large numbers may be opaque due to its un-_fathomability_ given that a human agent cannot possibly hope to work through each binary operation the program performs. However, it still maintains the properties of tractability and intelligibility. DNNs seem to disregard themselves in regards to tractability.

![[Pasted image 20250926104216.png]]

Burrell (2016): “[DNNs] are opaque in the sense that if one is a recipient of the output of the algorithm (the classification decision), rarely does one have any concrete sense of how or why a particular classification has been arrived at from inputs.

Creel 
Creel extends these concepts of opacity and transparency by providing three ways in which an algorithm can be opaque. 


Sogaard
The common arguments for DNN opacity refer to the status of either model size, continuity, nonlinearity, instrumentality, or incrementality (Sogaard). Due to the nature of DNN construction, as a instrument heavily reliant on orderings of training data, Skogaard claims that DNNs are opaque in regards to both training and prediction. Naming these two types of opacity training and inference opacity respectively. 

Boge makes a similar distinction between h(ow)-opacity, which concerns how a DNN alters its function in response to training data, and w(hat)-opacity which concerns what function was learned in the course of training. 

However, is this really opaqueness? 

(What are the different ways DNNs can be opaque?) Opaque in regards to how it arrived to a prediction and the lack of explanation along with the prediction. 

___

In treating the problem of opacity within DNNs, we will start with Humphrey’s (CITE) characterisation. He defines epistemic opacity as such:

“Here a process is epistemically opaque relative to a cognitive agent X at time t just in case X does not know at t all of the epistemically relevant elements of the process. A process is essentially epistemically opaque to X if and only if it is impossible, given the nature of X, for X to know all of the epistemically relevant elements of the process”

Humphreys epistemic opacity means that certain processes can be opaque to one agent but not to another. For example, the functioning of a calculator may be opaque to a philosopher but not to an electrical engineer.

However, this seems to present certain problems when viewed in relation to most scientific instruments. As Louis Bucciarelli (1994, Thing Knowledge pg.13) points out “Do you know how your telephone works?” (p.3, Designing Engineers). He explains that while one scientist might be able to explain one particular aspect of a telephones functioning (for example, how sound is produced by an electric current), they might not be able to parse the exact functioning of the algorithms employed in noise suppression (Cite Baird). Therefore, they are unable to fully ensure that the telephone is functioning as intended due to a lack of technical know-how, making it opaque. This presents a general problem for most scientific discovery since every scientist utilizes tools they are unfamiliar with. For example, a biologist in the process of recording their results may use the data analytics tools of a spreadsheeting program that is technically opaque to them.

Similar to this, is the concern that scientists are constantly forced to rely upon previously conducted work which they cannot verify the accuracy of. Even if it was the norm for a scientist to conduct a thorough investigation into the results he cites (an unrealistic practice due to social barriers), he still might face problems of opacity if the work employs tools which are technically unintelligible to him. Scientific results that are produced out of large organized groups, such as the large hadron collider (LHC) or LIGO, do not have a single agent who understands every epistemically important part (Rolin 2020, Miller & Freiman 2020; Longino 2022.)

CITATIONS ARE IN KOSKINEN

Given the varied and distributed system of scientific research, large elements of trust are required as it’s impossible for an individual to double check and fully understand all the previous information he relies on. Research, especially those of large groups, produce work in which no singular agent can interpret each moving part. Hardwig (1985, Koskinen) states that in cases like this, of collective knowledge production, trust stands in for justification. Granted that this trust is regulated in a few ways (Frost-Arnold 2013). Some informal, for instance the belief that your scientific peers are acting honestly, and some regulated, such systems of peer-review. These procedures of epistemic checking, when followed correctly, reduce error and the role of trust within knowledge production (Wilholt, 2013).

As established before, instruments cannot be trusted - they can only be relied on. Therefore, in cases of scientific instruments, trust is warranted as long as there is an agent who “understands how the instruments work, takes responsibility of them in an epistemically acceptable manner, and can be trusted” (Koskinen pg. 7). Returning to our example of the biologist, we can justify their usage of technically opaque instruments as long as there is an agent, such as the manufacturer, that exists. Results from large-scale scientific endeavors, such as the LHC, are justified on the basis that every part has an agent for which it is not epistemically opaque.

The reputation of DNNs as a “black box” means that there are no agents that can take responsibility due to its ‘opaqueness’. However, Next section.