Sources: 
[[Do Machine Learning Models Represent Their Targets?]]

Model-based explanations (or model explanations, for short) are explanations in which the explanans appeal to certain properties or behaviors observed in an idealized model or computer simulation as part of an explanation for why the (typically real-world) explanandum phenomenon exhibits the features that it does” (Bokulich, 2017, 104).

How do we justify models? 
How do we justify the reliability of a model? 

To recap: we have established that opacity results from an agent being unaware each epistemically relevant part of a system. However, we need to answer what advantage does being aware of the epistemically relevant parts of a system grant us? 

Structure
1. What are models? 
2. How do models represent their targets
3. Double nature of models 
4. What we require is a causal and conceptual account of a model 



What are models? 
As mentioned before, models are a diverse category and encompass both simple linear equations and large scale material models (Frigg and Hartmann 2020 SEP). In general, 'a model is an interpretative description of a phenomenon that facilitates access to that phenomenon’ (Bailer-Jones, 2009, 1). Furthermore, models are grounded and constructed within an existing body of scientific theory/knowledge. 

However, this explanation raises further questions. Firstly, how do models describe a given phenomena and how must this phenomenon be represented towards a human agent? Most accounts of models within scientific contexts focus on how the model represents a target phenomenon through, approximation, idealisation, or simplification (Weisberg 2013). The way in which the model is connected to its targeted phenomenon ($t_p$) could be mediated either by isomoprhic, structuralist, or mechanistic accounts among others. 

Depending on the specific nature of the model - whether it interacts materially, or performs numeric manipulations, on $t_{p}$ - the specific type of mediation will change. For example, if we assume an isomorphic relation between model M and $t_{p}$ then there is an element to element correspondence between parts of the model and the target system. 

Using Hooke's Law, for example, we can model a spring–mass system by using the equation ( F = -kx ). Here, the model elements (force ( F_m ), displacement ( x_m ), and spring constant ( k_m )) correspond isomorphically to the measurable features of a real spring system (( F_o ), ( x_o ), ( k_o )). The relations among these elements—the proportionality of force to displacement—are preserved across both sides.

This can be visualised as follows:
$$
[  
\begin{array}{ccc}  
F_m & \longleftrightarrow & F_o \  
| & \equiv & | \  
x_m & \longleftrightarrow & x_o \  
| & \equiv & | \  
k_m & \longleftrightarrow & k_o \  
\end{array}  
]

[  
r_m \equiv r_o  
]
$$
Where:
($\longleftrightarrow$) denotes the _isomorphic correspondence_ between the model and the real system.
($\equiv$) denotes the _equivalence of relational structure_ (i.e., how force depends on displacement through ( k )).

This is just one way that these relationships are expressed. Different models will have different ways of relating towards a target phenomena depending on how they are used. We can see that there is a bidirectional nature to models. The first is how they are related towards a target-phenomena, and the second is how these relationship is represented towards a human agent. Representations are useful to produce both explanations and understanding of a model and the model's target phenomenon. However, this raises certain problems, does a model need to be similar to its target phenomenon in order to be an accurate representation? (Mäki 2009; Giere 2004; Sullivan Models). We follow in Nguyen’s (2020) in accepting that a model has to be representation enough to allow for truthful inferences about the underlying phenomenon. What is required is that representations need to showcase their "essential directionality and its capacity to allow surrogate reasoning and inference" [[An Inferential Conception of Scientific Representation"]]. 

All models will encode a level of idealisation of the target phenomenon. Idealisation can be a simplification  of the target phenomenon or a purposeful omitting of some phenomenon. However, as long as an agent can trace a correspondence between the idealised element and the target, there are no real epistemic problems. [Gie10, Wei12, B+21, Duede models]. 

Before continuing, we have to acknowledge the double usage of the word explanation. Explanation can either be in reference to the underlying phenomena. I.e., the way that the model relates and represents the underlying phenomena allows for an agent to explain the underlying phenomena. The other usage of explanation is as an appeal to reliability. 

Let's take the example of a DNN, which is trained on the best data and has been correct thus far, that produces weather prediction. One day it predicts that there will be a large hurricane which requires immediate evacuation of the city, which will be both costly and disruptive. When agents are choosing to trust this result, they would hardly be satisfied by an explanation, given by an expert, which amounts to "it has been correct in the past". What they are seeking is a certain causal explanation of the DNNs reasoning.
Similar to a human weather forecaster, who would be able to describe the discrete steps in their reasoning when questioned. Other comparable statistical algorithms used for weather prediction were able to provide explanations by equating certain portions of weather data with a type of real-world phenomena. (Cite [[Conceptual challenges for interpretable machine learning]]). 





This type of epistemic demand is the same for other model instruments. What are the pre-requisites needed to justify the outputs of a model? 

The reliability of the model directly depends on how it represents the target phenomenon and how this information is communicated to a human agent. In seeking this representation we can defer to some results in the philosophy of science, where explanation can take many forms. Of interest to us is the causal mechanical (CM) model, which focuses on how models encode and represent the causal structure of the phenomenon they represent. (Salmon 1984, Erasmus) \Footnote{Deductive Nomological (Hempel and Oppenheim 1948), Inductive Statistical (Hempel, 1965), and NM (Machamer et al 2000) have very little use in application towards scientific instruments and decision making.}. 



This sort of explanation concerns the actual functioning and decision making of a DNN. Reliability, for *model instruments* requires an agent to be aware of these epistemically relevant in order to justify the result.
Therefore, opacity is the prevention of representation and understanding the higher-level rules of a DNN. This is why we have to reject an instinct to reduce our justification into a simple appeal to the models shifting weights and biases. This is one sense in which a DNN is a model, however explanations produced from this, such as "X neuron shifted its weight form 0.4 to 0.6 due to the result of a backpropogation algorithm which led to a prediction of hurricane" are not the type we are looking for. While they are causal, they are not conceptual in nature. Explanation requires a sense of semantic intelligibility that is acceptable by another agent. Therefore, what we are interested in is how a target phenomenon is encoded by a DNN and how this leads to a prediction. 

To back this up, we can look at other conceptions of opacity and transparency and see how the strongest notions of opacity all require the following CM model of explanation in order to prevent opacity. Zerilli argues for model opacity along the lines of linearity and dimensionality. A linear system with fewer dimensions is more fathomable than an alternate higher dimensional system. In which fathomability concerns a human observer who, in the former low-dimensional case, is able to “contemplate the entire model at once” (Lipton 2017, 4) (Zerelli, 7). An unfathomable system, for example, would be an extremely large computer simulation model with billions of parts. However, as long as this simulation maintains linearity, it retains another two of Zerelli’s properties - intelligibility and tractability. Tractability is whether a model can be run on a machine whereas intelligibility is if the relationship between a model’s subparts can be determined, despite size. Therefore, a large and complex model remains intelligible if an agent can trace the nature and relationship of the model’s constituent parts. For example, a computer program which multiplies large numbers may be opaque due to its un-fathomability given that a human agent cannot possibly hope to work through each binary operation the program performs. However, it still maintains the properties of tractability and intelligibility since the agent can abstract parts of the program to see how they causally relate to another. 

Both Creel (CITE) and Lipston (CITE) have raised distinctions along similar lines. However, instead of centring discussion around opacity, they evaluate a system in regards to three criteria of transparency. “Run” transparency, the first category, is the easiest to fulfil and requires the ability to survey the implementation code along with input data. The latter two categories – algorithmic and structural transparency – both pose problems for DNNs. Algorithmic transparency requires an agent to be aware of the high-level logical rules (which function) the model uses in the transformation of input to output whereas structural transparency requires an agent to understand how the architecture of a system encodes a specific function. In the case of DNNs, how the shifting mass of nodes and weights encodes a specific concept that, for example, identifies cats. 

To take stock, Zerelli’s fathomability and Creel’s run transparency seem similar and establish opacity by arguing that no human agent could familiarise themselves with each step. Within these classifications, the epistemically relevant parts of the program is each operation the computer performs at a hardware level. However, if this is the case then every computer program must be necessarily opaque and therefore un-reliable? For example, a simple program which takes the input of two numbers and returns their sum – if run on a modern operating system – will require billion of operations. Is this program opaque? According to Creel, it is run-opaque, but not algorithmically opaque because we are privy to the higher-level logical rules. An agent, when inspecting this program, has good reasons for abstracting certain parts of the system into concepts. An adequate knowledge of computer internals and assembly language allows them to justify a chain of causal reasoning regarding the program. They can claim that a certain line of code corresponds to a clump of transistors firing, justifying their reasoning through their knowledge of logic gates. If needed and given enough time, they could theoretically work through each binary operation to secure justification. Given that they can give good reasons for abstracting a certain set of operations into a certain function. E.g. this clump of transistors is responsible for encoding the character 'h' and interact with another clump which produces 'i' to output 'hi'.

If we are able to provide reasons for abstracting certain parts of a DNN (e.g. a set of neurons) into certain concepts, would we be able to remedy our problems with opacity? For example, if we return to our DNN which encodes the XOR function 

XOR DISCUSSION 

We can point to a neuron and give good reasons for why this represents one part of the XOR function, or how it fits into the overall function. There is an ability for an agent to point to a part of the model and link it towards a part of the target phenomena. 

At what point do we lose this ability? From here, we will investigate at what point a DNN is unable to provide this explanation compared to other transparent statistical models, such as linear regression or decision trees. To prove this will utilise Mill's method of difference in applying a certain property $\chi$ onto a transparent statistical algorithm and contrast this with a DNN to see if this is a sufficient condition for opacity. The main candidates for these properties are: size; complexity; non-linear nature; Fill in soon

___

Linear models are a type of statistical model that are defined in the following way: a target variable ( y ) is represented as a linear combination of input variables ( x_1, x_2, \ldots, x_n ), each weighted by a corresponding parameter ( w_i ), plus an error term ( \epsilon ). Formally,

$$
y = w_0 + w_1x_1 + w_2x_2 + \dots + w_nx_n + \epsilon.
$$

The model assumes that the expected value of ( y ) changes proportionally with the inputs. Meaning that the relationship between each input and the output is additive and independent of the others. During training, the model “learns” by adjusting the weights ( w_i ) to minimise some measure of error (typically the mean squared difference between the predicted and observed values). Why are these models considered transparent?

Specifically, we need to find out what part of opacity prevents an agent from understanding how a model's components relate to the target phenomena. 

DO OPACITY TO SHOW THAT THERE IS NO WAY TO ACTUALLY REPRESENT HOW DNN MODELS RELATE TO A TARGET PHENOMENA. 






Things only become opaque because of how they are encoded within the DNN system. 

It represents the point at which an agent is unable to give explanations for why an input is transformed into an output in a conceptual and causal way. The first question we must answer, in defending this formulation, is if DNNs encode concepts. 


As others have pointed out (Sullivan), there is a link uncertainty between the input and output of a DNN. However, this link uncertainty is created because of certain opaque features which a DNN possess. Continuing from Zerelli's and Creel's definitions of transparency, we can see that algorithimic opacity is a breakdown of explaining the higher level logical rules, i.e. the concepts of a model. As shown in our example, to justify reliability and trust in a result, we require a causal account of how this output was arrived at. Therefore, for a DNN to be justified as a model, it must provide a conceptual and causal account between input and out. 

===THEREFORE, a model can be opaque because of size because once a model gets larger it is harder to provide good reasons that certain parts of the model is doing X. ===

These properties are induced by the presence of a particular feature within the system. For example, a common feature that contributes to unfathomability is the size of the system. The underlying logic is this: a specific feature of the system prevents either algorithmic transparency (as discussed by Creel) or intelligibility (as argued by Zerelli), therefore making the system opaque. Numerous features have been proposed: model size, continuity, nonlinearity, instrumentality, or incrementality (Sogaard). 
However, are all of these equally sufficient conditions of opacity? If they are not, then how do we contrast any two properties and their effect on the opaqueness of a system? In attempting to answer this question, we can utilize statistical models which are considered to be inherently transparent. For example, decision trees. Decision trees are generally considered to be fully transparent algorithms (Mittelstadt et al., 2018, Skogaard pg. 227). They function as a nonlinear flowchart structure made up of nodes.






The representation of these targets, and the ability to run interventions on these causal variables, along with grounding within a certain theory. Allows for the creation of scientific explanation 


DNNs are a specific type of model, due to the architecture running as a computer program. 
Diagram 
Conceptual Model -> Simulation Model (Neurons and Biases) -> Computerised model (Transistors and Logic Gates) -> Actual Phenomenon. 

How does explanation arise from this phenomenon representing. 

Note that we will be working with two types of explanation: Explaining the functioning of a system and explaining the underlying phenomenon. 
 
Drawing from the philosophy of science literature on 

Types of models

What does this actually mean? How are they phenomenon targeted and representational? 

They are phenomenon targeted and representational 

How do we usually explain phenomenon and where do we go wrong with DNNs? 

Mills method of difference. At what point do we fail being able to represent a DNNs internal mechanisms? 

Opacity Arguments. 

Therefore, models need to encode concepts and present these concepts in a way to allow for reasoning and inference. Similar to causal mechanical (CM) model explanations in the philosophy of science. 

Doctor example. 

This is also why we can't justify DNNs just on their architecture, different from the T-DNN. Models require reasoning for how the input got to the output, but causal instruments require justification that the DNN is doing what is was meant to do. 

Do DNNs have concepts? 

Can these concepts be represented? 

They are not semantically decomposable 

Therefore, they cannot entirely be used to justify the reliability of a model. They can be used in an interventionist way to allow for people to do things with the underlying phenomenon (Bujisman)



