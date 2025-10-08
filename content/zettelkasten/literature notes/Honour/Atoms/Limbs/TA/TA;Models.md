TA: Counterfactual dependence [[Machine Learning models as Mathematics; interpreting explainable AI in non-causal terms]]

"Specifically in the case of ML systems there is then a range of different types of counterfactual dependence that we can be interested in when demanding explanations. Most technical explainability methods focus on the pattern of dependence of the output on the input. What would happen to the output were we to have a different input to the ML system?" 

What to add to? 

TA: 

""Model “goodness” should be judged by its accuracy with respect to existing empirical data, and its adequacy with respect to specific goals, not how close it comes to an unachievable and non-useful “ideal.” The assumption that if we could represent everything then we can achieve any and all of our goals is undoubtedly the intuition supporting completeness as an ideal. However, given we cannot represent everything, including more details in a model can be detrimental to both its accuracy (e.g. by over parameterizing in ways that compound uncertainty) and its adequacy (e.g. by obscuring main factors whose manipulation might be sufficient to meet the goal)." ""

TA: 
Concepts, 
What we are interested in is not the way in which certain parts of the model are cut up and linguistically named, but if this is even possible and what this means for interpretable models.

TA: 
Sullivan - Do ML models represent their targets.
If AI systems to not represent their targets, then they cannot be used for explanation 

Even if these models do not represent their targets in a way that is vulnerable to explanation. They are still able to be used for explanation 

TA: 

"**Patterns of Interpretability** The above models exhibit some common patterns of interpretability that are worth pointing out. The most important pattern of how we grasp a predictor seems to be a combination of two different means of grasping: First, the predictor function is grasped in virtue of the form of their representation (either the form of the predictor function itself or the form of the domain partition). Second, certain aspects, or parts, of this formal representation are grasped through visualization, or other modes of qualitative reasoning. These two steps are used in sequence, not in parallel; this can be seen most clearly in the case of GAMs and MARS, but also in the case of trees. Thus, one important lesson for interpretability gained here is that we grasp predictor functions not only by looking at their visualizations, but also by looking at their form, their symbolic representation." ML Interpretability: Simple Isn’t Easy Tim Raz 


TA:

From the point of view of human-machine communication, the most important issue concerning concepts is the issue of explanation [3, 5, 25]. If the scope is limited to individual concepts, it comes down to providing a transparent answer to the question why certain objects are recognized as concept referents and others are not. For example: an expert medical system that recognizes a patient’s symptoms as indicative of cancer should provide an explanation of why it suggests such a diagnosis. This is, in fact, an explanation “associated” with the concept of type N cancer encoded within the system. It should consist in showing some connection, convincing for a person (e.g., a doctor or a patient), between the observed symptoms and the suggested diagnosis (including indicating the symptoms that are relevant for the diagnosis). It turns out that, for some types of conceptual representations, such a connection is achieved naturally, while this is extremely difficult for others (see next section). [[Concepts as decision functions. The issue of epistemic opacity of conceptual representations in artificial computing systems]]

TA: 
"For, there are two ways in which DNNs could be associated with representations: They could (a) themselves be scientific representations, much in the same sense as traditional scientific models; or they could (b) be said to have representations, much in the same ways as humans and other animals do."

The weights and biases are not used by researchers to represent anything. What we are interested in is what the DNN itself holds in terms of representations. 

There are arguments that a DNN holds representations of a specific concept. 