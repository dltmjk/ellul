Write in introduction using instrument epistemology and applying it to DNNs. 

Epistemology of each type of instrument -> 

Show that Models section is contradictory
1. Epistemology of models 
2. Show that DNNs cannot fulfil these requirements 
3. ExAI also contradictory 

To DO: 
Explain methodology as shown above 
Structure according to methodology (e.g. Model requirements -> DNNs as a model)
Flesh out how representations are contradictory 
Flesh out ExAI part in regards to how they can provide an explanatory notion. 

===To add to Models section, continuing from our discussion on T-DNNs, why don't exai methods act in the same way as these pragmatic features. 

Because they are MODELS, their method of justification needs to be appealing to representational factors. NOT that if they can produce a desired output. 

They have this potential if they are integrated and tested, either through modifying the model to check the claims. However, the existence of an ExAI model alone does not confer reliability and accepting this is potentially dangerous. 

===TO ADD: ALSO Returning to our explanation of instrument which do not produce uninterpreted results. DNNs produce results that have to be understood in a certain 


==ExAI==
In an attempt to correct for this, multiple “Explainable AI” (ExAI) methods have been developed. These include salience maps \cite{simonyan2013deep}, local approximation techniques \cite{ribeiro2016why}, and layer-specific relevance analysis \cite{bach2015pixel}. Essentially, these methods all attempt to increase agent “trust” in ML systems by applying techniques to models that purport to explain their inner functionality.

For example, suppose we have a DNN that has already been trained and evaluated for its accuracy on a dataset, and that attempts to predict tumors within an MRI image. A post-hoc ExAI algorithm would generate an additional output that highlights, for each feature in the input image, how much that feature contributed to the overall classification.\footnote{This is an outline of how saliency maps work.} This localized relevance information is typically visualized as a heatmap, offering a glimpse into the internal processes of the model.

Such heatmap-based methods are part of the broader class of post-hoc explainability techniques, which assign an importance score to each input feature for a given input based on its influence on the model’s output. Visualizing these relevance scores produces the heatmaps that serve as explainable representations of the model’s behavior. While these methods are useful, we argue that they provide value only in somewhat elucidating the underlying phenomena; they do not provide arguments for reliability. They are reliable as models of a DNN, but not as models of the target phenomena itself.

Within ExAI, researchers often claim that their methods make the DNN more transparent \cite{simonyan2013deep}. However, ExAI does not modify any part of the DNN. Instead, it applies a separate algorithm to the DNN to produce a subsequent model. The example of a heatmap does not reveal any intermediate steps in the DNN’s prediction; rather, it is a separate model that takes the DNN as its target. An analogy can be drawn to computational neuroscience, where methods like representational similarity analysis (RSA) are used to study how the brain represents information. These methods take neural recordings and attempt to predict neural responses from stimuli or compare patterns of activity across regions. While they can show that a particular stimulus property correlates with neural activity, they do not demonstrate that the brain “uses” that representation in the same way the model does. In other words, they are models of the brain \cite{bo2025evaluatingrepresentationalsimilaritymeasures}.

If we evaluate ExAI techniques as models of a DNN, we can see that the methods employed in mapping the DNN are tractable and algorithmically transparent. Furthermore, the method of representation is clear to a human agent. Therefore, ExAI models are reliable models of a DNN. However, if an ExAI model is a model of a DNN, which itself is a model of a phenomenon, can we claim that an ExAI model is a model of the relevant phenomena? While this may seem convincing at first glance, it fails because DNNs remain opaquely related to their target phenomena. This means that we cannot draw a direct link between ExAI models and our object of scientific investigation. As Rudin \cite{rudin2019stopexplainingblackbox} claims,

\begin{quote}
	“If the explanation was completely faithful to what the original model computes, the explanation would equal the original model, and one would not need the original model in the first place, only the explanation.” \cite[p.~3]{rudin2019stopexplainingblackbox}
\end{quote}

If ExAI methods help in establishing certain features of the underlying DNN, can an agent appeal to these reasons in explaining the functioning of the DNN? This seems like a legitimate claim to make, given our formulation of opacity. Furthermore, as explored in our T-DNN section, if appeals to reliability can occur by appeal to epistemically relevant elements outside the system, then what prevents the ExAI model from serving as a reason for reliability? Similarly, why can't we classify ExAI methods as a type of pragmatic method?

This is because a model instrument is not a causal instrument. Model-based reasons for reliability require a causal formulation linking input and output and a representation of this process. An agent can justify a causal instrument through pragmatic methods because the epistemic demands are different. The epistemically relevant elements of a model will always be on the “inside.” For example, a neuroscientist can theorize about the function of the brain and collect experimental results, but the mere collection and modelling of this data would not count as a reason for the reliability of the underlying phenomenon. A comparable analogy would be: “We can relate the feeling of fear to the amygdala; therefore we can guarantee that the amygdala will function reliably when exposed to fear-inducing sensations.”

Some might argue that a post-hoc ExAI model can make genuine claims about the target phenomena because most human explanations of scientific processes are equally post hoc \cite{Hatherley478}. For example, a study by Bilalić et al. \cite{bil} showed that explicit explanations from researchers were post-hoc reconstructions rather than actual reports of their decision-making. However, cases of this sort are still troublesome, given that in the majority of cases we have no choice but to accept these statements due to how common they are. Furthermore, just because agents behave and accept such behaviours does not mean that we can justify similar epistemic reasoning in the case of instruments \cite{Alvarado2023-ALVSSC}.

Despite this, even if these ExAI models do not recreate the causal reasoning of their target DNN entirely, they can highlight future avenues of investigation. Rudin pejoratively claims that ExAI techniques do “not explain anything except where the network is looking” \cite[p.~5]{rudin2019stopexplainingblackbox}. That is, we are informed that a model encodes a feature, but not how this feature interacts with others in the dynamics of the model. Any attempt to infer this interaction is reasoning on top of the model, rather than a result produced by the model. While this is true, where the network “looks” may still be of importance. For example, it has been argued that DNNs can detect features within input data that are “not transparent to human researchers” \cite[p.~1]{Boge2023-BOGFCP-2}.

If this is the case, then ExAI methods can be integrated into a context of investigation which can, provisionally, provide hypotheses about the target phenomena — especially because these second-order models are transparent and reliable. These claims, in order to be justified, must be empirically verified in order to actually provide understanding. Buijsman \cite{Buijsman2022-BUIDEA} proposes that feature-identification allows us to create counterfactual cases for model behaviour, dissolving certain explanatory confusion\footnote{towards a target phenomenon}. For example, by revealing certain patterns or biases within the input data.

An important caveat of this approach is that these models cannot be employed as a standalone justification of the underlying DNN process. Claims of this sort would take the form of statements such as “this model has had ExAI techniques applied to it” as a reason. Yet, as we have shown, these techniques do not change anything about the underlying DNN model or its epistemic position. Furthermore, such claims may be used to give undue epistemic justification to certain models and displace the rigour that is required \cite{rudin2019stopexplainingblackbox}. The consequence is that unreliable models are falsely, and confidently, justified in high-stakes situations.

Conclusion. 
The argument of this paper proceeds as follows. First, we claim that DNNs are a type of scientific instrument, and their epistemic demands should therefore be treated on a par with those of other instruments. Second, we diagnose confusion surrounding the opacity of DNNs as stemming from a failure to distinguish their two distinct functions. Third, we apply the epistemic demands of causal instruments and model instruments separately to these two functions. Fourth, we conclude that in the case of T-DNNs, opacity can be offset by appeal to pragmatic and method-learning strategies. Finally, in the case of deployed DNNs, we show that opacity creates significant reliability problems and then evaluate ExAI techniques in this light, concluding that ExAI models may function as tentative theories that stand in need of empirical validation.



==To DO: why exai can provide hypotheses that can be tested===


This ability of ExAI models to show which features the DNN considers important allows for a glimpse of understanding. While explanation is not fully provided, researchers can use this as groundwork for further scientific investigation. It is important to note that scientists are only provided with information about what the DNN considers important—not why it considers this feature important. Similarly, ExAI methods do not reveal how a DNN actually utilizes these features to produce a prediction.

Certain approaches “test” the model with sets of input data to show that certain subsets of neurons are more active given the presence of specific features. However, the previous problems associated with the distributed nature of a DNN persist. We are given information about the location of certain features, but not how different features interact. That is, we are informed that a model encodes a feature in a certain place, but not how this feature interacts with others in the dynamics of the model. Any attempt to infer this interaction is reasoning on top of the model, rather than a result produced by the model. Due to our lack of epistemic access to the DNN’s representations, the second-order ExAI model is unfalsifiable. Therefore, we cannot achieve the relational understanding required to justify the model’s reliability.





We can return to our analogy of the brain. 



Some might argue that a post-hoc ExAI model can make genuine claims about the target phenomena because most human explanations of scientific processes are equally post hoc. This works as an argument for using ExAI as a springboard for further research, but not as a defense of the reliability of the underlying DNN. By highlighting which features the DNN considers most important, the ExAI model provides valuable information about potential avenues for scientific discovery.


Furthermore, it is dangerous the results of these models as reasoning for trusting the underlying DNN. 
