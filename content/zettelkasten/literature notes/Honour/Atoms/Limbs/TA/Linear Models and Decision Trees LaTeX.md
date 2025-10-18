\subsection{Linear Models and Decision Trees}
\subsubsection{Linear Models}
Linear models are a type of statistical model that are defined in the following way: a target variable ($y$) is represented as a linear combination of input variables ($x_1, x_2, \ldots, x_n$), each weighted by a corresponding parameter ($w_i$), plus an error term ($\epsilon$). Formally,
$$
y = w_0 + w_1x_1 + w_2x_2 + \dots + w_nx_n + \epsilon.
$$

The model assumes that the expected value of ($y$) changes proportionally with the inputs. Meaning that the relationship between each input and the output is additive and independent of the others. During training, the model “learns” by adjusting the weights ($w_i$) to minimize some measure of error (typically the mean squared difference between the predicted and observed values). Why are these models considered transparent?

First, an agent has good reasons for assigning certain meanings to the model parameters and these model parameters are easy for an agent to intuitively grasp. Second, the output is easily calculable, due to it being a result of additivity. Therefore, each input will always result in the same, traceable, change in output for the entire model \cite{R_z_2024}. This also means that there is no interaction between input variables. 

\begin{figure}[h]
\centering
\includegraphics[width=6cm]{linearmodel.png}
\caption{A Linear Model Visualized \cite{hastie01statisticallearning}}. 
\label{fig:XOR}
\end{figure}

\subsubsection{Decision Trees}
Decision trees are another type of interpretable model. Formally, a decision tree recursively partitions the feature space $\mathbb{R}^n$ using a sequence of decision rules of the form $x_j \leq t$, where $x_j$ is a feature and $t$ is a threshold. At each node, the algorithm selects the feature and threshold that maximize a chosen criterion, such as information gain (for classification) or reduction in variance (for regression). The model predicts the output $y$ by traversing the tree from the root to a leaf based on the input vector $\mathbf{x} \in \mathbb{R}^n$.

For example, a decision tree could be used in medical diagnostics to predict whether a patient has a disease based on features like age, blood pressure, and cholesterol levels, using a method analogous to a sequence of conditional statements. The tree might first split on whether the patient’s age is over 50, then on whether cholesterol is above a certain level, and so on, eventually leading to a classification of “disease" or “no disease" \cite{hastie01statisticallearning}.

Decision trees are considered transparent along similar lines. They are intuitively graspable thanks to the semantic labeling of each feature, which makes every decision performed by the model conceptual in nature. Furthermore, each decision is a binary one and each result is traceable given the input. 

\begin{figure}[h]
\centering
\includegraphics[width=8cm]{decisiontree.png}
\caption{A Decision Tree Visualized \cite{hastie01statisticallearning}}. 
\label{fig:XOR}
\end{figure}

Both linear and decision tree models are highly idealized and, importantly, allow their conceptual, phenomenon-directed features to be extracted easily. Especially in the case of decision trees which have their representations presented semantically (e.g. if age > 65 $\rightarrow$ retiree). 

\subsection{Opaque Models}
Does size present any problems for this conceptual nature? For example, given a linear model with billions of parameters, we are still capable of describing certain partitions of the model as corresponding to specific parts. In a large linear regression used for predicting house prices, for instance, we can still interpret the contribution of each feature (e.g., location, number of rooms, or proximity to schools) by examining its associated coefficient. Even if the model contains billions of such parameters, each still has a direct conceptual counterpart. Will the same hold for a decision tree? It seems only possible in cases where large chunks of the model can be separated into certain functional roles. However, certain decision trees can consist of billions of distinct else-if statements, which decreases the likelihood of this.

The same concern applies to DNNs. If our example of the XOR function were extended to a billion parameters, the ability to demarcate certain sections as corresponding to a particular function would decrease. Still, with a decision tree, it is possible for an agent (given enough time) to work through each binary operation and come away with an understanding of the model’s decision-making process. Unlike this, DNNs do not represent their parameters with any semantic description; they consist entirely of weights and biases (i.e., numbers). Furthermore, they lack any sort of “translation procedure” that can turn these into semantic features \cite{Buckner2019-BUCDLA}.

Therefore, we face two problems with DNNs compared to other statistical models. The first is that, given the immense size and complexity of these systems, an agent will have a hard time parsing and demarcating parts that correspond to specific, phenomenon-directed concepts. The second is that DNNs cannot benefit from having immediately and semantically graspable features. One could argue that, similar to the case of decision trees, an agent could work through each parameter operation to generate some understanding. However, as we will show, this is impossible, as any explanation of internal functioning will be underdetermined due to the distributed nature of DNN architecture.

\subsection{Distributed Models}

As Duede \cite{duede2025representationalstatusdeeplearning} identifies, DNNs are distributed in a way that presents certain problems. He shows that, due to the nature of a DNN’s layers and neurons all being activated in a feed-forward manner, information cannot be localized within individual units; that is, certain parts of the network do not selectively activate for individual concepts. The entire network is used because each layer depends on the previous one. This phenomenon becomes standard as DNNs grow increasingly large and complex. Therefore, each neuron participates in representing numerous input-output associations. Representational content, consequently, is not attached to a single parameter or node but is distributed across the system. Altering any one weight perturbs the activity of many others. In this sense, the deep network’s knowledge of its target is not localized in subparts, but rather distributed across the global configuration of interrelations among all its parameters.

One could argue that a network’s layers begin by “capturing” particulars before collating these into higher-level abstractions. For example, a neural network that recognizes dogs abstracts certain pixels into features such as a “nose” or an “ear.” This seems intuitively appealing, given the forward-facing architecture of a DNN. However, in order to prove this, an agent must provide good reasons for whether a DNN actually processes and produces features in this way. The immediate challenge lies in showing how certain types of input data can be broken down into “particulars.” Then, they would have to provide reasons for how these coalesce into specific features. In effect, this type of explanation only makes sense if we commit to a particular-to-abstract conception of DNNs.

Given this, the existence of DNNs that deviate from the standard “feed-forward” architecture by allowing neurons to “feed back” (i.e., to affect the value of previous layers) serves as a strong counterexample. If a network were linearly progressing toward the expression of certain abstractions, then each layer would necessarily be an abstraction of the last. If a layer is able to feed back into its “particular” ancestors, then this presents an obvious contradiction.

Any argument that appeals to the representative capacity of layers fails, because such approaches are underdetermined \cite{duede2025representationalstatusdeeplearning}. An agent simply lacks sufficient evidence to demonstrate the validity of one procedural process over another, given the absence of semantic signposts within DNNs and overwhelming size. It is reasonable to believe that the system captures and encodes certain aspects of the original input. However, given the scale of these distributed networks, these aspects do not appear to be locally encoded but rather globally (albeit in small parts).

\begin{figure}[h]
\centering
\includegraphics[width=13cm]{linear.png}
\caption{The Logistic Growth Equation Versus a DNN implementing the same function}. 
\label{fig:dnnfunction}
\end{figure}

An agent inspecting the system does not have any watertight reasons to select subsets as corresponding to a particular function. This is because every parameter within the DNN contributes to representing all aspects of the system, and representational meaning is fully global. Changing a weight at any point in the system has consequences for the entire system \footnote{Even in a feed-forward network since the previous nodes have to be re-calibrated to allow for the new weight value}. If the criterion for fully justifying a model is the ability to point to a subset and give good reasons for why it encodes a certain function, then the holistic nature of a DNN means that we do not have a proper epistemic reason to believe that any particular subpart fully encodes a specific function. This prevents an agent, unlike with other models, from being fully confident about how the DNN represents relationships between specific causal concepts.

Therefore, algorithmic reasoning does not appear in discrete chunks but rather through the functioning of the system as a whole. An analogy can be drawn with the brain, which operates in a similarly distributed manner. If we did not have direct epistemic access to the representations within our own brains (through conscious awareness), an agent would have no good reason to designate specific parts as corresponding to particular functions. However, if we were able to access the representations within a DNN, we could justify its functioning in the same way that we justify certain results in neuroscience. As we will see in the next subsection, this is precisely what the field of “Explainable AI" seeks to accomplish.

To recount: models require an agent to be able to demarcate subparts and assign them semantic meaning in order to provide both explanations and reasons for reliability. DNNs can do this at exceptionally small scales, as shown in our XOR example. However, as DNNs become increasingly holistic at larger scales, agents are unable to give watertight reasons for assigning meaning to any specific subparts. 