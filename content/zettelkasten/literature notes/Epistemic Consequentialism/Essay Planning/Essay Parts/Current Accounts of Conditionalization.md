Since our formulation of credences follows the probability axioms, it should also be answerable to other Bayesian norms. Specifically, conditional probability. Given a proposition $X$ we can calculate its probability given a proposition $E$ in the following way: 

$$P(X \mid E) \overset{\mathrm{df}}{=} \frac{P(X \& E)}{P(E)}.
$$
Applied to credences we get the following norm: 

$\textbf{Conditionalization:}$ If a subject with credences $\text{Cr}(\cdot)$ gets evidence $E$, they should adopt new credences $\text{Cr}_{E}(\cdot)$ such that $\text{Cr}_{E}(\cdot) = \text{Cr}(\cdot \mid E)$. 

This is a standard formulation of conditionalization. Let's say you start with a set of credences $\text{Cr}_{old}(\cdot)$ then you have *conditionalized* on $E$ when $\text{Cr}_{new}(\cdot) = \text{Cr}_{old}(\cdot \mid E)$ van Fraassen (1999). Joyce (2009) gives his account in the following way: 

"Imagine a person whose state of uncertainty is characterized by a "prior" probability $P_0$ on $\Omega$, and who is not dogmatic about $x$, so that $1 > P_0(x) > 0$. If the person undergoes a learning experience in which the only new information she acquires is that $x$ is certainly true, then her post-learning "posterior" probability $P_1$ should coincide with her pre-learning probability conditional on $x$, $P_1(\bullet) = P_0(\bullet|x)$." Joyce (2009, pp 419) 

One common issue with this version of conditionalization is that we must assign $E$ a credence of 1 and update all of our other credences accordingly. However, there are multiple cases in which our evidence might be uncertain. For example, observing something in less than ideal lighting or being told information by a friend known to lie. In these cases our evidence should not be treated the same as if it was told to us by a trustworthy friend. 

Given this, other normative constraints were proposed. Jeffrey (1965) advances a "generalisation" of conditionalization that defines evidence as a *partition* of propositions that sum to 1. In which the prior and posterior credence functions are defined on the same algebra $\mathcal{F}$:

$\textbf{Jeffrey Conditionalization:}$ If a subject $i$ with prior credences $\text{Cr}_i(\cdot)$ receives evidence that leads them to assign new credences to a partition $E = \{E_1, E_2, E_3, \dots\}$ of the probability space, then they should adopt revised credences $\text{Cr}_{i,E}(\cdot)$ such that:

$$\text{Cr}_{i,E}(\cdot) = \sum_j \text{Cr}_i(\cdot \mid E_j) \cdot \text{Cr}_{i,E}(E_j)$$

Jeffrey gives the following example:  

"The agent inspects a piece of cloth by candlelight, and gets the impression that it is green, although he concedes that it might be blue or even (but very improbably) violet. If G, B, and V are the propositions that the cloth is green, blue, and violet, respectively, then the outcome of the observation might be that, whereas originally his degrees of belief in G, B, and V were .30, .30, and .40, his degrees of belief in those same propositions after the observation are .70, .25, and .05. (Jeffrey, 1965, p. 154)"

This solves our problem of unreliable credences. However, a missing piece of our formulation has been the times in which an agent receives $E$ (Formally: $t(E)$) and at which point they adopt $E$ (Formally: $t(Cr_{e})$). In this case 'receiving' or 'getting' evidence is the point at which $E$ becomes epistemically relevant to our agent. Different versions of conditionalization have different answers to this question. The most popular are the posterior solution, and the concurrent solution. 

$\textbf{Posterior: }$ $t(Cr_{e})$ should be some time $t$ after $t(E)$.  (Earman 1992), Howson & Urbach 2006
$\textbf{Concurrent: }$ $t(Cr_{e})$ should be the same time as $t(E)$. Lewis 2010, Strevens 2015

In these interpretations $E$ is a partition of propositions that you receive over an interval of time, adopting $E$ is only possible at the end of this interval. However, this partitioning of evidence presents a few problems. 

Firstly, as Meachem (2015) points out, why exactly should we wait until the end of the interval before updating our credences? If we consider two agents, one who updates his credences immediately and one who waits until $E$ is complete at some time $t$, then it's hard to justify why our former agent would be worse off. Generally, it seems more epistemically rational to immediately update our credences given any partition of $E$. 

The obvious objection against this is when we learn something that might be untrue. 

This leads onto our second objection, can all evidence necessarily fit into an interval? There are cases in which $E$ is never "completed", in other words it is an open interval. 


Problems with this that our thing will fix for 
1. Credal reallocation
	1. Why does Jeffreys not work? 
2. Credal Reallocation events
	1. Memory Loss
	2. Awareness growing 
	3. Fallibilism 
3. Context-Sensitivity 
	1. Old Evidence 
	2. Uncertainty 

Credal Reallocation Event






We don't believe that evidences every really scale into 1, or that evidence can be bounded. 




conditionalization problems 
1. Time of Proposition
2. Memory Loss
3. Awareness Growing
4. Old Evidence
5. Context-Sensitivity 

We need to explicate 
1. When to update beliefs
2. How beliefs should be updated
3. How beliefs should be structured 
	1. Modelling uncertainty!!!

Causal connection between certain propositions. We believe X because of Y. Can we model this? 



Evidence is changed from a proposition to a set of propositions with a corresponding weight. $E = \set{(E_{1}, X_{1}), (E_{2}, X_{2}), (E_{3}, X_{3},\dots)}$. $E_{1}-E_{N}$ are mutually exclusive and jointly exhausive. The weights are in the $[0-1]$ interval and sum to 1. 
