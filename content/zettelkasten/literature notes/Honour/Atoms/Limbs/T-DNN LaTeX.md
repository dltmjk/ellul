===Edited out===
We argue that T-DNNs, as a type of causal instrument, can be epistemically justified for reasons that are not obscured by algorithmic opacity. 

To demonstrate that this holds, we first need to delineate the actual function of the T-DNN.


===LaTeX===
\subsection{Opacity and T-DNNs}
The type of opacity relevant to DNNs is algorithmic opacity. Authors who have previously distinguished between the training and deployment stages focus on how the conditions of opacity differ between them. Boge \cite{Boge2021-BOGTDO-4} introduced two ways in which a DNN can gain $\chi$. He makes a distinction between h(ow)-opacity, which concerns the way in which a DNN automatically alters the instantiated function in response to data, and w(hat)-opacity, which concerns what function was learned in the course of training.

Søgaard \cite{Sgaard2023-SGAOTO} makes a similar distinction between inference and training opacity. The former relies on a human agent being unable to relate input and output, whereas the latter arises when a human agent “cannot, upon inspection, say how, in general, the parameters of the DNN were induced as a result of its training data" \cite[p.~225]{Sgaard2023-SGAOTO}. Both Boge and Søgaard argue that the opacity of the training process presents problems for reliability. 

However, if we can confer reliability on a causal instrument based on purely structural transparency, then can we not do the same for DNNs? This seems intuitively appealing: if a T-DNN is the same type of instrument as a microscope, then the epistemic demands of both should be equal. The causal chain of the T-DNN is as follows: the network’s layers, activation functions, and optimisation process collectively constitute its “working parts.” When properly constructed and trained, these components interact to produce stable mappings from input to output across a range of data. The code implements these features on a computer, and because programming languages are structurally transparent, so is the T-DNN. While constructing the model, the T-DNN identifies features within the input space and fits certain patterns inherent in the data.

The immediate problem is that we cannot reduce the theory-dependence of a T-DNN in the same way we can with a microscope. A microscope relies on the laws of optics, whereas a DNN relies on the results of statistical learning theory (SLT). The more important theory, as Boge \cite{Boge2021-BOGTDO-4} asserts, is the one that the T-DNN “realizes” in constructing its function. Our lack of epistemic access to this theory is an important caveat that limits our reliance on such systems. If reliability can only be conferred when an agent has knowledge of this theory, then opacity presents serious problems.

One might attempt to deflate the epistemic significance of the T-DNN by characterizing it merely as a generic function approximator, arguing that the particular function it learns is irrelevant so long as it learns some function. If we accept this, then we would require only structural transparency to justify the use of the T-DNN. However, this view is untenable, since the epistemic and practical utility of DNNs does not stem from their capacity to approximate arbitrary functions but from their ability to identify specific, meaningful ones. Moreover, the fact that a T-DNN can sometimes learn the wrong function also presents problems for reliability.

Examples include adversarial attacks and overfitting. Adversarial attacks describe a phenomenon in which DNNs are vulnerable to “deceptions” \cite{papernot2016practical, goodfellow2015explaining, szegedy2014intriguing}. For instance, certain DNNs can “cheat” their way through classification. Consider a neural network trained to classify MRI images as containing a tumour or not. Suppose that, in the training data, scans showing tumours were disproportionately captured under certain lighting conditions or scanner settings (e.g., brighter room lighting or particular scanner gain). The network might then learn to associate brightness or shading artefacts with the tumour label—in other words, it recognises lighting conditions rather than actual tumour morphology \cite{athalye2018synthesizingrobustadversarialexamples}. Similarly, overfitting occurs when a model fits too closely to the training data, thereby preventing generalisation. Would access to the higher-level rules governing a DNN’s training resolve this issue?

The answer is broadly yes, which is why both Boge and Søgaard argue that epistemic access to the T-DNN’s realized function is necessary to secure its reliability. Moreover, if opacity prevents an agent from inspecting this realized function,\footnote{We assume this for now and discuss it in detail in Section~6.} how can we possibly justify the training stage? While these are genuine concerns, we argue that they can be mitigated if an agent is able to provide alternative grounds for justifying a system’s reliability. Such grounds follow from a form of method-learning advanced by Kieval and Westerblad \cite{kieval2024deep}.

\subsection{Pragmatic Understanding}

Inspired by Dewey’s view that methods emerge “organically” from successful inquiry and then serve as standards for future work, this sort of scientific know-how implies that the reliability of the T-DNN stage depends on epistemically relevant elements—apart from the model itself—that grow out of scientific practice. Method-learning, and its constituents, provide a way for agents to justify the reliability of an instrument. Instead of appealing to a wholly transparent argument, agents appeal to methods such as design rules and other epistemic strategies for justifying reliability.

\begin{quote}
“We know that some methods of inquiry are better than others in just the same way in which we know that some methods of surgery, farming, road-making, navigating or what-not are better than others.” \cite[p.~108]{Dewey1938-DEWLTT}
\end{quote}

In a similar vein, Lenhard \cite{Lenhard2019-LENCSA-4} argues that, in the case of an opaque computer simulation, agents can grasp the mechanics of a system through its action rather than through its theoretical backbone. These reasons are practical in nature and emerge from experimental contexts, “even when the dynamics [of an instrument] have not been grasped in theoretical terms” \cite[p.~171]{Lenhard2019-LENCSA-4}. This kind of pragmatic understanding appears to challenge our earlier formulation of opacity. However, we must remember that opacity poses problems for reliability only when an agent is unable to explain how a particular result was reached. Epistemic relevancy refers to the components of explanation that an agent employs to justify that result.

Model instruments are useful because they function in analogy to a given phenomenon and therefore require a degree of internal interpretability to fulfil their epistemic role. In contrast, causal instruments detect relationships within or between phenomena. If an agent can appeal to epistemically relevant facts that demonstrate an instrument’s capacity to perform this function on a desired target, these should count as adequate reasons for reliability. Moreover, it does not matter whether the reasons an agent provides in justifying a result appeal to factors “inside” (e.g., higher-level rules) or “outside” (e.g., experimental contexts, method-learning) the system, as long as they serve to justify the output. Both types of reasons, being epistemically equivalent, can confer reliability.

Therefore, if an agent can implement systems that render the DNN reliable across multiple contexts, these constitute valid epistemic reasons for its reliability. We can also say that the contexts in which an instrument is used contribute to the justification of its results. Building on this idea, let us return to the problem of adversarial attacks. Consider, by analogy, a compass used in a scientific experiment. We expect it to detect the Earth’s magnetic field; however, other strong magnetic forces may interfere. The compass is doing precisely what it was designed to do (detect magnetic fields) but it may still yield misleading results depending on its context of use. This is analogous to a DNN, which identifies a particular function based on patterned features within the input data. It is impossible to guarantee that it will always capture the correct function, since what counts as “correct” may vary with context. Similarly, a researcher might attempt to use a compass to measure the magnetic field of an object in another room rather than the Earth’s field. In both cases, the researcher can justify that the instrument is identifying the correct field—or function—by appealing to the circumstances of use.

One might object that such reasons are valid only because they rely on the transparency of the instrument. Namely, that all reasoning about reliability is epistemically dependent on knowledge of an instrument’s internal functioning. However, in the case of contexts of use, we need only appeal to a form of structural transparency rather than algorithmic transparency. For example, a common requirement for training DNNs is to ensure that the training and deployment data satisfy the i.i.d. assumption. This means that the data points are independent and identically distributed. Properly selected input data increases reliability by appealing to SLT. In essence, when the i.i.d. assumption holds, researchers can provide a principled basis for trusting the T-DNN's reliability \cite{vonluxburg2008statisticallearningtheorymodels}.

Generally, examples like this appeal to the “robustness" of a system \cite{grote}. Other causal instruments are justified on similar grounds. For example, nuclear magnetic resonance (NMR) spectroscopy occupies a special epistemic position because the phenomena it interacts with are not observable outside the results produced by the device \cite{mitchell}. Consequently, reasons pertaining to its reliability can appear circular.

\begin{quote}
“Instead, instrumental reliability is supported by the stability of instrumental results in different places and times using the same experimental protocols (replicability) and stability of results among very different kinds of experiments (reproducibility or convergence)." \cite[p.~37]{mitchell}
\end{quote}

In our previous case of tumor classification, a greater variety of training data could rectify the error. The medical‑imaging literature is alert to this: artifacts (scanner noise, motion blur, background gradients) are known to be confounders and are often controlled or corrected in preprocessing or artifact‑removal pipelines \cite{vandergoten2022widerangemriartifact}. For the reliability of the training stage of the DNN, we only need to defer to the contexts of its experimental use. What we are interested in is identifying the correct pattern. To increase the likelihood of this occurring, researchers can utilize, for example, varied training data.

These are all valid reasons that can be given for the increased reliability of a model. However, these differ in nature from our type of “method-learning" since they can appeal to certain theoretical results. These pragmatic strategies are grounded in past experience which gave rise to epistemic strategies. They are actions taken which have consistently led to better models in the absence of any theory. 

If we return to our AlphaFold example, the training process was guided by expert knowledge of biological constraints, which were encoded as inductive biases and geometric constraints rather than by theoretical principles of protein folding. One such example is the implementation of "recycling," which fed back predictions from another model order to refine the training stage \cite{alphafold2020}. Similar to this was the implementation of multi-sequence alignments  

MSA is a bioinformatics technique that involves comparing a protein's amino acid sequence against a database of evolutionarily related sequences. The core idea is that when a mutation occurs in one part of a protein, compensatory mutations often arise in another part to preserve the protein's functional three-dimensional structure. When implementing this, the DeepMind team chose a self-attention mechanism because it intuitively captures the long-range, pairwise dependencies across a sequence. This implementation led to a notable improvement in performance.

However, some might worry that this is just a camouflaged appeal to reliability based on past success. While this is partly true, as researchers do appeal to accuracy as a measure of model performance, this practice is an unavoidable feature of scientific discovery and doesn't detract from the fact that these methods can still confer reliability. For AlphaFold, we do not have access to a direct theory of protein folding. Therefore, the only way to measure reliability is through this sort of accuracy measurement, rather than adherence to a theory.

Boge and Søgaard are correct in identifying that opacity presents notable problems. We grant that full epistemic access to the DNN would make questions of reliability relatively straightforward. Still, we can provide reasons that appeal to pragmatic considerations and offer similar justification. While both approaches are similar in conferring reliability, our pragmatic approach still precludes questions of explanation. This is another important caveat of DNN usage and will be covered in relation to models in our next section.




These methods were applied only appealing to the structural transparency of a system. 

However, some might worry that this is just a camouflaged appeal to a reliability on past success. While this is partly true, since researchers will appeal to accuracy as a measure of model performance. However, this is an unavoidable feature of scientific discovery and it doesn't detract from the fact that these methods can still confer reliability. 

However, these methods give rise to an important explanatory role that exonerates them from this concern. For example, 

We add X -> model gets better at Y. Therefore X and Y are causally related. 


===To add to Models section, continuing from our discussion on T-DNNs, why don't exai methods act in the same way as these pragmatic features. They have this potential if they are integrated and tested, either through modifying the model to check the claims. However, the existence of an ExAI model alone does not confer reliability and accepting this is potentially dangerous. 

===TO ADD: ALSO Returning to our explanation of instrument which do not produce uninterpreted results. DNNs produce results that have to be understood in a certain 


In essence guiding the the DNN to produce certain results. 

In this way the DNN becomes a type of phenomenon that is being experimented on. 







___

If we return to our AlphaFold example, the training process was guided by expert knowledge of biological constraints \cite{alphafold2020}, which were encoded as inductive biases and geometric constraints rather than by theoretical principles of protein folding. This sort of steering of a DNN’s architecture allows an agent to argue, with evidence, for the reliability of its predictions. These predictions do not depend on transparent reasoning but on the successful articulation of methods that mediate learning. The model’s epistemic legitimacy, then, parallels that of a scientific instrument whose calibration is maintained through expert practice. 

To sum: while access to a T-DNN’s higher-level ‘decision-making’ process would be useful, we can give good reasons for the reliability of a T-DNN without appealing to it. Some may prefer explanations referring to the former, taking the form “the DNN used this feature because it has x relevancy.” Other explanations, for example those pertaining to the input data, such as “our model shows robust performance in an i.i.d. setting” \cite{grote}, work equally well.

However, they do not explore any alternative ways an agent can justify a system’s reliability. We contend that an agent can offer reasons for trusting the reliability of a T-DNN without appealing to these higher-level rules. In other words, an agent may have good grounds for claiming that a T-DNN realizes a particular function even without direct access to it.



Let's assume that opacity prevents an agent from inspecting the realized function \footnote{We will cover this in detail in section 6}. 




Still, this highlights something important about the usage of DNNs.  



The causal chain of the T-DNN is as follows: The network’s layers, activation functions, and optimisation process collectively constitute its “working parts.” When properly constructed and trained, these components interact to produce stable mappings from input to output across a range of data. The code implements these features on a computer, and because programming languages are structurally transparent, so is the T-DNN. While constructing the model, the T-DNN identifies features within the input space and fits certain patterns inherent in the data.

When justifying the reliability of a normal causal instrument, we provide explanations that refer to how its subparts interact. It is important to note that these explanations do not rely on any higher-level rules but are grounded solely in the architecture of the system. Why, then, would an explanation that invokes only the structurally transparent features of the T-DNN fail?

The argument is that a T-DNN 

The answer is broadly yes, which is why both Boge and Søgaard argue that epistemic access to the T-DNN’s realized function is necessary to secure its reliability. However, they do not explore any alternative ways an agent can justify a system’s reliability. We contend that an agent can offer reasons for trusting the reliability of a T-DNN without appealing to these higher-level rules. In other words, an agent may have good grounds for claiming that a T-DNN realizes a particular function even without direct access to the realized function.




Correct experimental context
- Causal Instrument - Magnet 
- Correct input data and expert knowledge 


Furthermore, reasons given by an agent to explain why a certain output was produced often refer to circumstances outside the functioning of the system. For example, if you want to explain why a spectrometer produced a certain output, you would appeal to the input data. A T-DNN is, after all, a tool that minimizes loss in relation to input data. If we can give reasons that support the consistency of this function, we can sustain accounts of reliability. We acknowledge that access to its “decision-making” process would enhance explanatory potential, but reliability can still be conferred with or without this feature. 

Returning to our problem of adversarial attacks. Let's consider a compass produced and utilized within a scientific experiment, we hope that it picks up on the Earth’s magnetic field. However, other strong magnetic forces may interfere. The compass is doing what it was produced for - picking up on a magnetic field. This is similar to a DNN, which picks up on a certain function based on patterned features within the input data. It is impossible to control that it will pick up on the correct function every time because the context of what the “correct" function is will change. Similar to if a researcher wants to use a compass to measure the magnetic field of an object in another room, instead of the Earth's. Similarly, the microscope is a magnifier; what it actually magnifies is variable. Adversarial attacks and overfitting would cause problems with reliability if there was no way to shift these contexts of use. Fortunately, causal instruments and DNNs, both have other methods which confer reliability. 

In our previous case of tumor classification, a greater variety of training data would be able to rectify the error. The medical‐imaging literature is alert to this: artifacts (scanner noise, motion blur, background gradients) are known to be confounders and are often controlled or corrected in preprocessing or artifact‐removal pipelines \cite{vandergoten2022widerangemriartifact}. For the reliability of the training stage of the DNN we only need to defer to the contexts of its experimental use. What we are interested in is picking up on the correct pattern. In attempting to increase the likelihood of this occurring, researchers can utilize pragmatic statistical and scientific methods. It's important to note that these methods do not require any appeal to algorithmic transparency in the T-DNN. They function, and can be justified, on the basis of structural transparency (i.e., the parameters of the DNN)