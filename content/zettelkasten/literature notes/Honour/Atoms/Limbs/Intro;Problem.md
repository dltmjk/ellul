Structure: 
1. DNN usage across scientific fields 
	1. Alphafold example 
2. How are DNNs used across scientific fields (raising the question of experiment or instrument)
3. Scientists have two main problems with DNNs
	1. They do not provide explanations of the underlying mechanism 
		1. Explanation being the clarification or discovery of new knowledge within science. 
	2. They are "epistemically opaque", or "black boxed"
4. Structure of the paper

Sources:
[[On scientific understanding with artificial intelligence]]



REWRITE THIS 
"his paper focuses on models based on DNNs, because these have been responsible for the most impressive successes in recent years and because they pose the most interesting challenges from an epistemological point of view. However, we will occasionally consider also other ML methods, such as Logistic Regression (LR) and Random Forest (RF) models as they share some features of DNN models and some features of traditional scientific models. For the sake of concreteness, we focus on supervised ML models for binary classification. However, everything discussed in this article could be easily extended to other models of supervised ML. Unsupervised ML methods have quite different purposes and are beyond the scope of this paper." ([[Reliability and Interpretability in Science and Deep Learning]])

===Field Examples===
DNNs have been employed in multiple different scientific fields. For example,

They have been heralded as 
"Popular-level accounts even go so far as to proclaim a “revolution in scientific research” (Royal Society and Alan Turing Institute, 2019, p. 1), or that DNNs are “changing the way we do science”." [[Two Dimensions of Opacity and the Deep Learning Predicament]]

"anthrax spores (Jo et al., 2017), to calculate phenotypic distances from butterfly photographs (Cuthill et al., 2019), to improve breast cancer diagnostics (Witowski et al., 2022), to monitor urban earthquakes (Yang et al., 2022), in materials science (Zhong et al., 2022), and so on." [[On the Opacity of Deep Neural Networks]] 

More examples: 
DeepMind’s application to problems in healthcare (Fauw et al. 2018), deep learning models for data reduction in high energy physics (Guest et al. 2018) and bias in autonomous systems (Danks and London 2017).

The use of artificial intelligence (AI) for decision-making has become widespread. This includes banking (Aggarwal, 2021), criminal recidivism (Dressel & Farid, 2018), hiring (Kuncel et al., 2014), policing (Alikhademi et al., 2022) and healthcare (Alowais et al., 2023; Gulshan et al., 2016; Donnelly, 2017; Longoni, Bonezzi and Morewedge 2019; McKinney et al., 2020; Topol, 2019). Baron, trust explainability and AI. 

===Black Box===
DNNs have faced allegations of being "black boxes" (Find Citations). This is a common, if not colloquial, label for a tool that transforms input into output without allowing an agent access to its its method.

DNNs, in comparison to other machine learning models, are exceptionally successful. However, as some researchers have pointed out, this increased predictive capacity seems to carry with it a greater level of "opaquness". Some claim that that “machine learning provides us with ever increasing levels of performance, accompanied by a parallel rise in opaqueness" [[Prediction versus understanding in computationally enhanced neuroscience]] (Omri Barak (2017: p. 5)

===Original Bringing up of Opaqueness===
Opaqueness refers to "epistemic opacity" which was originally coined by Humphreys (CITE) to describe certain computer simulations in which the"epistemically relevant" parts are unknown (Humphreys pg. X). These definitions, along with their consequences and application to DNNs, will be explored in greater detail later. Researchers raise two main problems with the black box or opaque nature of DNN usage. Firstly, their "black box" nature limits the ability for agents to understand what logic is being followed between input and output which prevents trust. Secondly, this opaque nature prevents any explanation of the phenomena they model. 

===Explanation and Trust=== 
The first claim is based around an argument that DNNs are epistemically precarious position due to some property they possess which makes them *opaque* to an agent. While numerous of these properties have been proposed (size, non-linearity, and lack of grounding have all been considered and will explored later). Each one, if they are actually sufficient to induce opacity, will produce issues with trust. This concern extends from a widely held belief that trust is necessarily contingent on a level of explainability. The claim is that "Explainability is ... a pre-requisitefor practitioner trust. (Dam et al., 2018, p. 53)" and  "In order for humans to trust black-box methods, we need explainability ... (Gilpin et al., 2018, p. 80)". Opaqueness, in preventing explanation also prevents trust.  

Due to this opacity, the DNN acts as an oracle which predicts accurately without any subsequent explanation. If scientists are unable to provide explanations for certain outputs then this presents serious concerns, especially when these tools are applied in high-stakes situations such as criminal justice or medical use (Falco Governing AI Safety 2021). FOOTNOTE{Specify that this analysis is not just for scientific contexts, it is for everything. While our analysis concerns itself mostly with DNN usage within medical or scientific discovery usages, the arguments advanced are fully general and can be extended to apply to DNN usage within loan-making or criminal recidivism. [[Criminal DNN]]}

Transparency is useful both for justifying the results of a model but also for the construction of explanations regarding an underlying phenomenon, which is our second concern. 

===Example of Explanation vs Understanding=== 
This worry motivated by the fact that "Many standard applications of deep learning [...] focus on prediction. [...] Scientific applications, on the other hand, are often focused on understanding—identifying underlying mechanisms giving rise to observed patterns in the data." (Raghu and Schmidt 2020, p. 27)

This can be illustrated by example: 

The CASP, short for \textit{"Critical Assessment of Structure Prediction"}, is a worldwide biennial protein-structure prediction competition. Contenders, usually large research groups, are given a set of modelling targets – proteins for which the structure has not been determined in the form of an amino acid sequence – and must predict the structure. A protein is, structurally, a sequence of amino acids. When a protein interacts with other molecules, it \textit{folds} into a set 3-dimensional structure. During his 1972 Nobel speech, Christian Anfinsen theorized that this 3D structure was somehow encoded within the 1-dimensional amino acid sequence and that the former could be determined from the latter. The \textit{protein-folding} problem concerns \textit{why} a certain amino acid sequence will lead to a certain protein structure and what physical law this transformation follows. \citep{proteinfolding}.\\

Progress was exceptionally slow and traditional modelling techniques, such as *ab initio* methods, were the only prediction techniques that showed any promise. This was until the 13th CASP competition, at which a DNN dubbed 'AlphaFold', designed by Google's DeepMind team, outperformed every traditional model and took first place. Predicting structures to a nearly 90% accuracy. Specifically, AlphaFold2 achieved a median backbone accuracy of 0.96 Å, while the next best method had a median accuracy of 2.8 Å. This means that AlphaFold's predictions were, on average, within about the width of an atom from the actual protein structures, approximately 2.9 times more accurate than the next best method \citep{Jumper2021}. 

Since then, Alphafold has produced a data-bank of almost every protein structure known in nature \citep{alphafold2020}. However, it operates without ever "explaining" its predictions. 

As one scientist (Greg Bowman, director of Folding@home) points out:
AlphaFold doesn’t explain how proteins fold, which is another important piece of the protein folding problem. [...] There are also a host of related problems, such as what sort of moving parts do folded proteins have? How do these dynamics enable proteins to transmit information and cargos? How can we design drugs to turn proteins off (or on)? How can we design proteins to perform new functions? [[Minds and Machines]] pg. 2

In comparison, traditional modelling techniques, while less accurate, helped in explaining certain sub-problems related to protein-folding. For example, determining the hydrophobic effect (minimising contact with polar water molecules during protein construction) as a major driving force of protein-folding. ===Researchers were able to tinker with these algorithms, implement safeties and counterfactuals, and examine exactly why certain starting conditions manifest into particular results===. For example, changing energy states at specific times allowed researchers to understand exactly how a specific structure was simulated. Every predicted protein had a unique \textit{why} even if it did not assist in solving the larger problem \citep{MUNOZ1996R71}. 

This tension between prediction and explanation is common with DNN usage in science. As Boge (2022 Two Dimensions) states: 

"Many standard applications of deep learning [...] focus on prediction—learning to output specific target values given an input. Scientific applications, on the other hand, are often focused on understanding—identifying underlying mechanisms giving rise to observed patterns in the data"

While AlphaFold has increased our data on protein folding, it hasn't allowed for the construction of a general, underlying, theory. Raz and Beisbart (2022, pg. 12) argue that scientific discovery should aim for an "objectual understanding" of a subject matter or phenomenon. In this case of AlphaFold, the goal would be to encourage a greater understanding of the "the protein universe", which necessitates answering questions such as: "why do proteins fold in this manner". 

DNNs do not provide explanations along with their predictions. Due to this, scientists 'would not be entirely satisfied because they would want to comprehend how the [DNN] made these predictions' [[On scientific understanding with artificial intelligence]]. Sullivan (CITE) describes this as the 'link-uncertainty' of a model. In which “the amount, kind, and quality of scientific and empirical evidence supporting the link connecting the model to the target-phenomenon" is unknown. 

This discrepancy between AlphaFold and traditional models forces us to ask where the qualitative difference is? 










Read: 
[[On scientific understanding with artificial intelligence]]



Neither can we rely on purely inductive considerations when justifying our trust in DNNs, due to the opacity of the system.

We present the different classifications of scientific instruments in an attempt to highlight the common features present in each. We show how instruments always are constructed within certain contexts, either in view of a theory or in the context of an experiment.

We establish that scientific instruments need to fulfill certain considerations in order to be considered reliable in regards to an agent evaluating the system. The lack of any agent who can guarantee the reliability of a system poses problems when utilising the system in scientific contexts. DNNs due to their “black box” nature, or opacity, mean that they are unable to fulfill this criterion of reliability towards any agent.



Our Solution 
DNNs should be treated similarly to other instruments in which explanation is only provided in the backdrop of a theory, or if a DNN is particularly engineered for a specific use. Experiment-design (investing x by allowing the dnn to perform y which can be interpreted in z way) allows them to become explanatory 

DNNs, being universal function approximators, grants them substantial prediction power within scientific use. This function is present somewhere within the training architecture (weights and biases) of the network but is not given explicitly to an agent. Inducing what many call 'epistemic opacity' into the system and making these systems less 'understandable' than other similar, but purposefully created, experimental apparatus developed in the past. 

Our analysis does not include cases in which DNN outputs can be independently verified – rendering any concern about opacity redundant (Duede, 2022).



