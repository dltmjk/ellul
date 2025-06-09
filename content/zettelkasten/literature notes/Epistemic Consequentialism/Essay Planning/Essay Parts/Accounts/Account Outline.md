#### Directed Acyclic Graph (DAG)
Formalization: Let $G=(V,E)$ be a **directed acyclic graph** where $V=\{X_{1},\dots ,X_{n}\}$ is a finite set of random-variable nodes and $E\subseteq V\times V$ is a set of directed edges such that $G$ contains no directed cycles.

Parents : $\mathrm{Pa}(X_{i})=\{X_{j}\mid (X_{j},X_{i})\in E\}$ 
What is Anc and Desc? 
   * $\mathrm{Anc}(X_{i})$ and $\mathrm{Desc}(X_{i})$ are defined by reachability along the arrows.

Philosophical Rationale: 

**Markov Condition** (Pearl, 2009; SGS, 2000)
$$
     P(X_{1},\dots ,X_{n})=\prod_{i=1}^{n} P\!\bigl(X_{i}\mid \mathrm{Pa}(X_{i})\bigr)
   $$
Every variable is probabilistically independent of its non-descendants, given its parents. 

**d-Sepeartion**
A path $\pi$ between two variables is **blocked** by a conditioning set $Z$ iff
	(a) $\pi$ contains a chain or fork $A\!\rightarrow\!B\!\rightarrow\!C$ or $A\!\leftarrow\!B\!\rightarrow\!C$ with $B\in Z$; or
	(b) $\pi$ contains a collider $A\!\rightarrow\!B\!\leftarrow\!C$ where neither $B$ nor any descendant of $B$ is in $Z$.
Variables $X$ and $Y$ are **d-separated** by $Z$ iff all paths between them are blocked.
	⇒  If $X$ and $Y$ are d-separated by $Z$ then $X\!\perp\! Y\mid Z$.

**Interventions (do-operator).**
$\text{do}(X=x)$ cuts incoming edges to $X$ and sets it exogenously.
   $$
     P(Y\mid \text{do}(X=x)) \;=\; \sum_{v\setminus\{X,Y\}} \!
               \Bigl(\prod_{Z\neq X} P(Z\mid \mathrm{Pa}(Z))\Bigr)_{X=x}
   $$
This distinguishes **causal** from purely evidential influence.

