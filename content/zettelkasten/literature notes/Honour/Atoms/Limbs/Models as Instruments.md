Sources: 
[[Do Machine Learning Models Represent Their Targets?]]

What exactly are the higher level rules needed 

1. What are models 
2. How do we justify models 
3. Why can't we justify DNNs
4. Why ExAI does not justify the DNN but only explains it 
5. This can be used to provide further analysis of the underlying mechanism 
6. But does not act as an reason for justifying reliability 

===Section Outline===
This section establishes that an agent can justify the output of a model if they can:
1. Understand how the model relates to its target phenomenon; and
2. Explain which parts of the model correspond to specific aspects of the phenomenon.
We then show that this type of relationship is impossible for DNNs due to their distributed nature. We also evaluate ExAI methods to determine whether they can resolve these issues. We conclude that, while ExAI methods provide explanatory value, they do not confer reliability on a DNN.


===What are models? ===
Models are a diverse category and encompass both simple linear equations and large scale material models (Frigg and Hartmann 2020 SEP). We can return to our previous definition where 'a model is an interpretative description of a phenomenon that facilitates access to that phenomenon’ (Bailer-Jones, 2009, 1). We need to add that models are grounded and constructed within an existing body of scientific theory/knowledge. 

However, this explanation raises further questions. Firstly, how do models describe a given phenomena and how must this phenomenon be represented towards a human agent? Most accounts of models within scientific contexts focus on how the model represents a target phenomenon through, approximation, idealisation, or simplification (Weisberg 2013). The way in which the model is connected to its targeted phenomenon ($t_p$) could be mediated either by isomoprhic, structuralist, or mechanistic accounts among others. 

Depending on the specific nature of the model - whether it interacts materially, or performs numeric manipulations, on $t_{p}$ - the specific type of mediation will change. For example, if we assume an isomorphic relation between model M and $t_{p}$ then there is an element to element correspondence between parts of the model and the target system. 

Using Hooke's Law, for example, we can model a spring–mass system by using the equation ( F = -kx ). Here, the model elements (force ( F_m ), displacement ( x_m ), and spring constant ( k_m )) correspond isomorphically to the measurable features of a real spring system (( F_o ), ( x_o ), ( k_o )). The relations among these elements (the proportionality of force to displacement) are preserved across both sides.

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

This is just one way that these relationships are expressed. Different models will have different ways of relating towards a target phenomena depending on how they are used. We can see that there is a bidirectional nature to models. The first is how they are related towards a target-phenomena, and the second is how these relationship is represented towards a human agent. Representations are useful to produce both explanations and understanding of a model and the model's target phenomenon. However, this raises certain problems, does a model need to be similar to its target phenomenon in order to be an accurate representation? (Mäki 2009; Giere 2004; Sullivan Models). 

We follow in Nguyen’s (2020) in accepting that a model has to be representation enough to allow for truthful inferences about the underlying phenomenon. What is required is that representations need to showcase their "essential directionality and its capacity to allow surrogate reasoning and inference" [[An Inferential Conception of Scientific Representation]]. All models will encode a level of idealisation of the target phenomenon. Idealisation can be a simplification  of the target phenomenon or a purposeful omitting of some phenomenon. However, as long as an agent can trace a correspondence between the idealised element and the target, there are no real epistemic problems. [Gie10, Wei12, B+21, Duede models]. 

Before continuing, we have to acknowledge the double usage of the word explanation. Explanation can either be in reference to the underlying phenomena. I.e., the way that the model relates and represents the underlying phenomena allows for an agent to explain the underlying phenomena. As Bokulich explains:

> Model-based explanations (or model explanations, for short) are explanations in which the explanans appeal to certain properties or behaviors observed in an idealized model or computer simulation as part of an explanation for why the (typically real-world) explanandum phenomenon exhibits the features that it does” (Bokulich, 2017, 104).

The other usage of explanation is as an appeal to reliability. As Morrison (1999, p.63) expresses: 

> "The reason that models are explanatory is that in representing [their target] systems they exhibit certain kinds of structural dependencies. The model shows us how particular bits of the system are integrated and fit together in such a way that the system’s behaviour can be explained"

Let's take the example of a DNN, which is trained on the best data and has been correct thus far, that produces weather prediction. One day it predicts that there will be a large hurricane which requires immediate evacuation of the city, which will be both costly and disruptive. When agents are choosing to trust this result, they would hardly be satisfied by an explanation, given by an expert, which amounts to "it has been correct in the past". What they are seeking is a certain causal explanation of the DNNs reasoning.

Similar to a human weather forecaster, who would be able to describe the discrete steps in their reasoning when questioned. We are seeking a statement along the lines of "clouds of this type are always associated with hurricanes". Other comparable statistical algorithms used for weather prediction were able to provide explanations by equating certain portions of weather data with a type of real-world phenomena. Furthermore, if an agent is able to map on the relevant representations of the DNN onto the real world, they would be able to glean important information about the behaviour of the phenomenon. (Cite [[Conceptual challenges for interpretable machine learning]]). 

Within the philosophy of science this is known as the causal mechanical (CM) type of explanation, which focuses which focuses on how models encode and represent the causal structure of the phenomenon they represent. (Salmon 1984, Erasmus) \Footnote{Deductive Nomological (Hempel and Oppenheim 1948), Inductive Statistical (Hempel, 1965), and NM (Machamer et al 2000) all have little use in the case of DNNs. \cite[[Deep Neural Networks as Scientific Models]]}. 

===Justifying model reliability===

If we accept this then, if a model can represent a phenomena in a way that allows for reasoning, we can make claims about a phenomena based on the model. However, this is all contingent on the fact that the model actually represents the target phenomena in a way that allows for this type of explanation. I.e., an agent must have good reasons for showing that a subpart of a model (e.g. $F_{m}$) actually corresponds to a phenomenon (force). If they are able to provide this, then they must further furnish their explanation with a causal and conceptual account of how a model went from input to output. 

Our need for a conceptual model is why we have to reject cannot appeal to reliability based only structural transparency. This is one sense in which a DNN is a model, however explanations produced from this, such as "X neuron shifted its weight form 0.4 to 0.6 due to the result of a backpropogation algorithm which led to a prediction of hurricane" are not the type we are looking for. While they are causal, they are not conceptual in nature. Explanation requires a sense of semantic intelligibility that is acceptable by another agent. Fong and Vedaldi give their explanation of a DNN output in the following way: 

> An explanation is a rule that predicts the response of a black box $f$ to certain inputs. For example, we can explain a behavior of a \textit{robin} classifier by the rule  $Q_1(x; f) = \{ x \in \mathcal{X}_c \leftrightarrow f(x) = +1 \},$ where $\mathcal{X}_c \subset \mathcal{X}$ is the subset of all the robin images. Since $f$ is imperfect, any such rule applies only approximately. We can measure the faithfulness of the explanation as its expected prediction error: $\mathcal{L}_1 = \mathbb{E}[1 - \delta_{Q_1(x;f)}],$ where $\delta_Q$ is the indicator function of event $Q$. Note that $Q_1$ implicitly requires a distribution $p(x)$ over possible images $\mathcal{X}$. Note also that $\mathcal{L}_1$ is simply the expected prediction error of the classifier. Unless we did not know that $f$ was trained as a robin classifier, $Q_1$ is not very insightful, but it is interpretable since $\mathcal{X}_c$ is (Fong \& Vedaldi, \citeyear{FongVedaldi2017}, p.~3450).

While this is an accurate breakdown of a DNNs function, it does not give us insight to how parts of the DNN relate to the phenomena in question (robins). What we are interested in is how a target phenomenon is encoded by a DNN and how this leads to a prediction. Specifically, what type of causal methods are encoded by the DNN in actually identifying a robin. Like any model instrument, this requires an agent to be aware of the context that a DNN is situated within. Fon and Vedaldi's robin classifier only makes sense if we know that we are testing for a robin within a photo. For an agent to construct conceptual correlates of a DNN to the target phenomenon, they require this type of theoretical grounding. I.e., a DNNs architecture by itself will not tell you, in any conceptual way, what target phenomenon it is directed towards. Therefore, what we require is algorithmic transparency. 

If we return to our example of a program which outputs 'hi'. Algorithmic opacity was corrected by identifying certain components and assigning a conceptual function to this subpart. E.g. certain transistors were grouped together to encode the 'h' char. However, nothing about the transistors themselves would lead an agent to be aware of this function. This parallels our discussion of the construction of model instruments. Where theory both creates and grounds the model. This gives an agent good reasons for connecting the functioning of a model (and the output) with a certain theoretical, which allows them to privilege to apply certain concepts to parts of the model. 

This type of reasoning, originally pioneering within cognitive science research (CITE), have been extended towards DNN. Generally dubbed mechanistic interpretability (CITE), it is performed in the following way: 

1. Breaking the DNN into subparts. For example, singular neuron or sets of parameters
2. Conceptual labelling of the subpart. 

To illustrate this point, consider a DNN that represents the logical XOR function. A minimal network capable of learning XOR contains two hidden neurons, each of which can be shown to encode a subfunction analogous to logical operations such as “AND”, “OR”, or “NOT”. For instance, one neuron may activate when only one input is high. Which mirrors the behavior of a NOT gate composed with an AND gate. When visualized or analyzed through activation patterns, we can identify that this neuron corresponds to a conceptual component of the XOR function. 

[Diagram]
https://www.researchgate.net/figure/a-A-sample-DNN-to-learn-the-XOR-function-b-the-values-of-X-and-Y-according-to-the_fig3_359771176

What this demonstrates is that a DNN, even though realized as a distributed network of weighted connections, can encode _structurally meaningful subcomponents_ that correspond to elements of the phenomenon it models. In the case of XOR, these correspondences can be exactly mapped to logical relations. We can see that this DNN is not algorithmically opaque because we can point to a neuron and give good reasons for why this represents one part of the XOR function, or how it fits into the overall function. Which fulfils the criteria for model reliability. 

However, do we retain this ability in systems of extreme size? our XOR network is made up of a few hidden layers, whereas those in real scientific use contain billions. As we will see, this overwhelming size makes any demarcation of the model impossible. From here, we will investigate at what point a DNN is unable to provide this explanation compared to other transparent statistical models, such as linear regression or decision trees.

___

Linear models are a type of statistical model that are defined in the following way: a target variable ( y ) is represented as a linear combination of input variables ( x_1, x_2, \ldots, x_n ), each weighted by a corresponding parameter ( w_i ), plus an error term ( \epsilon ). Formally,

$$
y = w_0 + w_1x_1 + w_2x_2 + \dots + w_nx_n + \epsilon.
$$

The model assumes that the expected value of ( y ) changes proportionally with the inputs. Meaning that the relationship between each input and the output is additive and independent of the others. During training, the model “learns” by adjusting the weights ( w_i ) to minimise some measure of error (typically the mean squared difference between the predicted and observed values). Why are these models considered transparent?

First, an agent has good reasons for assigning certain meanings to the model parameters. Lipton (2018) refers to this as the decomposability of a model. Furthermore, these model parameters are easy for an agent to intuitively grasp. Second, the output is easily calculable, due to it being a result of additivity. Therefore, each input will always result in the same, traceable, change in output for the entire model. 

Decision trees are another type of interpretable model. Formally: a decision tree recursively partitions the feature space Rn using a sequence of decision rules of the form xj ⩽ t, where xj is a feature and t is a threshold. At each node, the algorithm selects the feature and threshold that maximizes a chosen criterion such as information gain (for classification) or reduction in variance (for regression). The model predicts the output y by traversing the tree from the root to a leaf based on the input vector x ∈ Rn.

For example, a decision tree could be used in medical diagnostics to predict whether a patient has a disease based on features like age, blood pressure, and cholesterol levels using a method similar to an else-if statement. The tree might first split on whether the patient’s age is over 50, then on whether cholesterol is above a certain level, and so on, eventually leading to a classification of "disease" or "no disease" (Quinlan, 1986).

Decision trees are considered transparent along similar lines. They are intuitively graspable thanks to the semantic labelling of the feature, making each decision performed by the model conceptual in nature. Both the linear and decision tree models are highly idealised and, more importantly, are prone to having their conceptual, phenomenon-directed features extracted easily. 

Does size present any problems for this conceptual nature? For example, given a linear model with billions of parameters, we are still capable of describing certain partitions of the model as corresponding to certain parts. In a large linear regression used for predicting house prices, for instance, we can still interpret the contribution of each feature (e.g. location, number of rooms, or proximity to schools) by examining its associated coefficient. Even if the model contains billions of such parameters, each still has a direct conceptual counterpart. Will the same hold for a decision tree? it seems only possible in cases where large chunks of the model can be separated into certain functional roles. However, certain decision trees can be made up of billions of else-if statements, all of which are distinct, the possibility of this decreases. 

The same concern is applicable to DNNs. If our example of the XOR function was extended to a billion parameters. The ability to demarcate certain sections as corresponding to a certain function decreases. In addition, unlike decision trees, DNNs do not represent their parameters with any sort of semantic description (i.e. it is all weights or biases - numbers). 

Furthermore, as Duede identifies, DNNs are distributed in a way which presents certain problems. He shows that, due to the nature of a DNNs layers and neurons all being activated in a feed forward manner, information cannot be localised within individual units. I.e., certain parts of the network do not light up for certain concepts. The entire network is used because each layer depends on the last. This phenomenon becomes standards as DNNs being increasingly large and complex. Therefore, each neuron is used in representing numerous input-output associations. Representational content, therefore, is not attached to a single parameter or node but is distributed across the system. Altering any one weight perturbs the activity of many others. In this sense, the deep network’s knowledge of its target is not encoded in subparts but in the global configuration of interrelations among all its parameters.

An agent, inspecting the system, does not have many good reasons for selecting subsets as corresponding to any function. This is because every parameter within the DNN participates to some degree in representing all contents, and representational meaning is fully global. If the criterion for fully justifying a model is the ability to point to a subset and be able to give good reasons for why it encodes a certain function. The holistic nature of a DNN means that we don't have a proper epistemic reason for believing that any particular subpart fully encodes a specific function. This stops an agent from being fully sure, as is the case with other models, how the model represents the relationship between certain causal concepts. 


===ExAI===
In an attempt to correct for this, multiple “Explainable AI” (ExAI) methods have been constructed. These range from salience maps (Simonyan et al. 2013, getting serious about), local approximating techniques (Riberito et al., 2016), and layer-specific relevance analysis (Bach et al., 2015). All of these methods all appeal to post-hoc explainability. 

For example, if we have a DNN, which has already been trained and evaluated for its accuracy against a set of training data, that attempts to predicts tumours within an MRI image. A post-hoc ExAI algorithim would generate an additional output that highlights, for each feature in the input image, how much that feature contributed to the overall classification \footnote{This is an outline of how saliency maps work}. This localised relevance information is typically visualised as a heatmap, which offers a glance into the internal process of the machine learning model.

Such heatmap-based methods belong to the broader class of post hoc explainability techniques, which, for a given input, assign an importance score to each input feature based on its influence on the model’s output. Visualizing these relevance scores produces the heatmaps that serve as explainable representations of the model’s behaviour.

While these methods are useful. We argue that they only provide value for researchers in somewhat elucidating the underlying phenomena but do not provide arguments for reliability. They are reliable as models of a DNN, but not as a model of the target phenomena itself. Despite this, it can still be used to increase scientific understanding.

Within ExAI, researchers claim that their methods make the DNN more transparent (cite). However, ExAI is not changing any particular part of the DNN. Instead, it is applying another type of algorithm onto the DNN to produce a subsequent model. The previous example of a heatmap is not revealing any intermediate steps in the DNNs prediction, instead it is a separate model which takes the DNN as its target.
An argument can be made by analogy to computational neuroscience. Methods like representational similarity analysis (RSA), which are often used to study how the brain represents information. These methods take neural recordings and try to predict neural responses from stimuli or compare patterns of activity across regions. While they can show that a particular stimulus property correlates with neural activity, they do not demonstrate that the brain “uses” that representation in the same way the model does. In other words, they are models of the brain. 

If we evaluate ExAI techniques as models of a DNN, we can see that the methods employed in mapping the DNN is tractable and algorithmically transparent (find source for ExAI DNN stuff). Furthermore, the method of representation is clear towards a human agent. Therefore, ExAI models are reliable models of a DNN. If an ExAI model is a model of a DNN, which itself is a model of a phenomenon, then can we claim that an ExAI model is a model of the phenomena? While prima facie convincing, it fails because DNNs are still opaquely related to their target phenomena. Meaning that we cannot draw a direct link between ExAI models and our object of scientific investigation. 

Some might argue that that a post-hoc ExAI model can make genuine claims about the target phenomena because most processes of human explanation of scientific explanation are equally as post hoc. This works as an argument for using ExAI as a springboard for further research but not as a defense for the reliability of the underlying DNN. In highlighting what features the DNN considers most important, the ExAI model is able to provide valuable information about further paths of scientific discovery. 

For example, it has been argued that DNNs are able to pick up on features within input data that is “not transparent to human researchers” (Boge FCP pg. 1). This ability for ExAI models to show what DNNs consider important features allows for a glimpse of understanding. Explanation is not fully conceded, but researchers can use this as groundwork for further scientific discovery. It’s important to note that scientists are only provided with what the DNN consider important – not why it consider this feature important. Similarly, ExAI methods do not grant us any insight into how a DNN actually utilizes these features to produce a prediction. 

Certain approaches “test” the model with sets of input data to show that certain subsets of neurons are more active given the abundance of a certain feature. However, our previous problems with the distributed nature of a DNN persist. We are given information about the location of certain features but not how different features interact. I.e., we are given information that a model does encode this feature in a certain place, but now how this feature interacts with others in the dynamics of the models. Any attempt to correct for this will be reasoning ontop of the model instead of a result given by the model. Due to our lack of epistemic access into the DNNs representations, the second-order ExAI model is unfalsifiable. Therefore, we cannot fulfill our requirement for a relational understanding in a model and use that to justify its reliability. 




ExAI is a model of the DNN, not a model of the phenomena
However, this model is reliable 
But, we cannot falsify ExAI because we do not have access to the DNN and we have no good way of proving that the DNN is accurately representing the phenomenon. 
Still, we can use this to lead to scientific investigation of further things. 
It adds a bit of explanation, not entirely, but allows us to see what features are important 
However, it does not add to reliability. 




While certain sets of neurons light up more than others. Due to this distributed nature we cannot say that that this subpart represents a certain phenomenon entirely. Only that this subpart is correlated with a certain phenomenon in our ExAI model. 

Similarly, ExAI is a model of the DNN. 



Furthermore, the way that it represents the DNN is not sufficient to believe that the DNN actually encodes representations this way - because of the previously discussed holistic nature. 



===How ExAI models engender objectual understanding but not trust. ===

Saliency maps show you what is relevant, but it doesn't tell you why this is relevant. However, being able to see what is relevant allows for a level of explainability. 

Why don't ExAI methods justify reliability? 

Because these methods are always post-hoc. We have no good reason to believe the a DNN actually encodes the representations the way we think they do. 

However, we can still construct good reasons to make a model of the DNN. A model of the DNN is a simplification of the DNNs functioning but adds to explanation. A model of the DNN is saying, this part of the DNN is x and that relates to y in the real world. And x is related to z, therefore we have good reasons for saying that x and z are related in the real world because of the inductive success of the DNN. This does not act as a claim in itself, but a claim in further need for research. DNNs can extend scientific research. 

What we are actually evaluating with this secondary model is the reliability of the methods of ExAI. We have good reasons for trusting this model because ExAI methods are fully transparent. 

We cannot trust the first DNN model because the methods used to connect phenomenon to target are shaky and uninspectable. 

However, ExAI creates a new model and connects this to the DNN model. Obviously, this does not justify a causal chain connecting the ExAI method to the actual phenomenon as the DNN model is still unsustainable. However, it allows for a degree of explanation and further research. 

ExAI -(reliable and inspectable)-> DNN -(not inspectable)-> phenomenon 

ExAI methods, as has been said, do not justify the reliability of the DNN, but only the reliability of the model constructed from the DNN, which can assist in explanation. DNNs, however, still remain uninspectable. Because there are no good reasons for saying that the DNN actually connects to the target phenomenon, compared to the reasons for saying that an ExAI algorithm connects to the DNN. 

In this way, the DNN becomes a type of phenomenon that the ExAI methods model. ExAI methods do not confer reliability to the actual DNN, but only to this secondary model. 





===These factors block the ability for an agent to evaluate how exactly the DNN acts as a model in reference to its target. ExAI methods are able to run empirical tests on these models to create evidence for certain parts representing certain functions. Therefore, providing a type of causal explantion. However, due to the unreliability of these methods in actually establishing the real representational capacity of a DNN. It cannot be an argument for reliability. However, it can assist in explanation. ===











Things only become opaque because of how they are encoded within the DNN system. 

It represents the point at which an agent is unable to give explanations for why an input is transformed into an output in a conceptual and causal way. The first question we must answer, in defending this formulation, is if DNNs encode concepts. 


As others have pointed out (Sullivan), there is a link uncertainty between the input and output of a DNN. However, this link uncertainty is created because of certain opaque features which a DNN possess. Continuing from Zerelli's and Creel's definitions of transparency, we can see that algorithimic opacity is a breakdown of explaining the higher level logical rules, i.e. the concepts of a model. As shown in our example, to justify reliability and trust in a result, we require a causal account of how this output was arrived at. Therefore, for a DNN to be justified as a model, it must provide a conceptual and causal account between input and out. 

===THEREFORE, a model can be opaque because of size because once a model gets larger it is harder to provide good reasons that certain parts of the model is doing X. ===

These properties are induced by the presence of a particular feature within the system. For example, a common feature that contributes to unfathomability is the size of the system. The underlying logic is this: a specific feature of the system prevents either algorithmic transparency (as discussed by Creel) or intelligibility (as argued by Zerelli), therefore making the system opaque. Numerous features have been proposed: model size, continuity, nonlinearity, instrumentality, or incrementality (Sogaard). 
However, are all of these equally sufficient conditions of opacity? If they are not, then how do we contrast any two properties and their effect on the opaqueness of a system? In attempting to answer this question, we can utilize statistical models which are considered to be inherently transparent. For example, decision trees. Decision trees are generally considered to be fully transparent algorithms (Mittelstadt et al., 2018, Skogaard pg. 227). They function as a nonlinear flowchart structure made up of nodes.






The representation of these targets, and the ability to run interventions on these causal variables, along with grounding within a certain theory. Allows for the creation of scientific explanation 





