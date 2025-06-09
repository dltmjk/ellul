1. Outline
	1. Formalizing a DAG (Directed acryllic graph) as found within causal modelling literature within Pearl (2009) and Spirtes, Glymour, and Scheines (2000). 
	2. How credences and evidence will be defined in this model. Taking inspiration from Causal Bayesian Networks. 
	3. How evidence will affect this DAG



	4. "Intervention" to prove causality, Ricola pg 1946
		1. It is impossible to explain the actual dynamics of causal relevance we can model it in this way 
	5. We can represent credal, or evidential sets with variables. 
		1. Why is it a probability distribution
			1. We follow from Weisberg and Pettigrew in allowed for credences to lie in the span of your possible future credences. 
			2. That is, if your current credence function is $c$ and your possible future credence functions are $c_1, \ldots, c_n$, then there should be $0 \leq \lambda_1, \ldots, \lambda_n \leq 1$ such that $\sum_{i=1}^{n} \lambda_i = 1$ and $c = \sum_{i=1}^{n} \lambda_i c_i$
2. How does this work 
	1. A credal reallocation event renders you certain of E
		1. In this case a credal reallocation event is defined in the following way: 
			1. General perception, whatever
			2. Memory Loss
			3. Self-Doubt
			4. Awareness. 
		2. You then conditionalize on E
	2. When should you conditionalize? 
		1. Seinfeld Paper
	3. 


3. Philosophical Backbone of Causality 
	1. Causal Structure Outline
		1. Prereq
			1. This might mean that the agent’s belief state is not just a flat list of probabilities, but a **structured model** (for example, a Bayesian network or some causal graph over propositions). 
			2. if evidence $E$ is observed, the update focuses on adjusting beliefs about $E$ and its **direct causes or effects** in the network, rather than free-floating adjustments. This idea is akin to Pearl’s **“locality”** – only update the nodes connected to the evidence, and let the effects propagate via known links
		2. Imprecise and incomplete credences are represented through a set of measures. 
			1. "This article presents a complete theory of credal networks, structures that associate convex sets of probability measures with directed acyclic graphs"
			2. $V_i$ is defined by an equation $V_i = f_i(\text{Parents}(V_i), U_i)$, where $U_i$ is an exogenous noise term
	2. How are weights updated? 
		1. Bayes rule or something else? 
		2. Posterior $p(w|D) \propto$ Prior $p(w)$ × Likelihood $p(D|w)$. In practice, exact inference is intractable for large networks, so researchers use **approximate Bayesian updating** techniques like _variational inference_ and _Markov Chain Monte Carlo_. **Variational inference (VI)** has been especially popular: it posits a flexible family of distributions $q(w|\theta)$ to approximate the true posterior and then **finds the parameters $\theta$ that make $q$ as close as possible to the true posterior**
		3. Typically this is done by minimizing the Kullback–Leibler (KL) divergence $D_{\mathrm{KL}}\big(q(w),|,p(w|D)\big)$, which measures the “information loss” in using $q$ instead of the exact posterior
		4. In effect, the BNN’s update finds the new belief distribution that is as **conservative a deviation from the prior** as possible while accounting for the data
	3. Factorized Belief State
		1. A BNN-inspired rule could take this further by using something like a **factorized belief state**: update modules of the belief network in a targeted way. For example, if our epistemic state includes beliefs about cause $C$ and effect $E$, learning $E$ should update our belief in $C$ _only to the extent that $C$ is known to influence $E$_, and not affect unrelated parts of the network. Formally, this could be achieved by conditionalizing on $E$ in the submodel concerning $C$ and $E$, while leaving other independent sub-beliefs unchanged (respecting a **causal version of Jeffrey’s rigidity condition**).
4. Gradual updating
	1. E as an input, 
		1. The new rule would generalize Jeffrey conditionalization by allowing any **degree of belief change in evidence** to propagate to other beliefs. Instead of requiring an update only when “$E$ is learned with certainty, the rule would take as input something like _“the agent’s credence in $E$ has changed from $p$ to $p’$. _’$.”_ The update to other propositions $H$ would then follow a **weighted adjustment**
		2. This could be implemented by an iterative procedure (analogous to gradient descent) that makes a **series of mini-conditionalizations** as the credence of $E$ moves from $p$ toward $p’$. Such a process would reflect **procedural rationality**, acknowledging that real agents may update in stages. Notably, this is conceptually similar to how a BNN learns: each data point or small batch nudges the distribution rather than causing an instantaneous full update.
	2. Conservatism in Credence changes 
		1. **minimizes change from the prior while accommodating the new evidence constraints**
		2. Principle of minimal change due to Diaconis & Zabell (1982, Section 5.1) and Dietrich et al. (2016)




Credal Reallocation Event: 

