## Ordering Items
Certain things can be ranked on a scale. For example, if A is preferred to be then A > B on a certain ordinal scale. This concept can be applied to certain epistemological notions like confidence. An example of this type of ordinal series is given here:

Imagine you prefer apples to bananas, we can express this in the following way:
$$ P_{ab}$$
We can also express a certain type of indifference in the same way. For example if you neither prefer bananas or grapes:
$$I_{bg}$$
Using this information we can construct a "ladder" of sorts which expresses these preferences in the aforementioned ordinal series. Since we know that A > B and B = G, then our ladder would hold two "rungs". The first contains apples and the second contains bananas and grapes. For these types of orderings to be valid, they have to hold the ability to be categorized in this way. 

Therefore, orderings cannot be circular. So we cannot have A > B > C > A. The following would be contradictory. Currently we only posses a series which orders but does not assign any sort of numerical value. By assigning certain numerical values to things (For example, lets say you like applies an amount of 6, but you only like bananas a 4) we can consider techniques of strategic dominance. 

## Terminology
The most common usage of strategic dominance is within game theoretic applications. However, strategic dominance can also be employed when making certain personal decisions (For example, what to buy for dinner given certain prerequisite information)

The common setup of most game theory problems is that there exists a set of players :$$\left\{ 1, 2, \ldots, n \right\}$$Each player $i$ has a set of strategies or moves they can make in a certain game state. Each move has a potential playoff, so if there are $m$ moves a player can make, there is an equivalent amount of payoffs. Lets say we have two strategies $A  \&  B$. 

$A$ **strictly dominates** $B$ $(A > B)$ if choosing A always results in a better outcome than choosing B regardless of what other players do. 

$A$ **weakly dominates** $B$ $(A ≥ B)$ if choosing A always gives *at least as good an outcome* as choosing B, no matter what the other players do. 

Using our previous example of apples and bananas, we can say that our strategy of picking apples (A) strictly dominates picking bananas (B) because our numerical values assigned to $A \& B$ justify the following relationship: $A > B$. These numerical values are our payoff values. Each strategy $s \in S_{{i}}$ has a payoff  $u \in U_{{i}}$. Each payoff is a real number which can be calculated given a certain strategy. This gives us the payoff function which is: $$ u_{i} : S_{{1}} \times  S_{{2}} \times \ldots S_{{m}} \rightarrow \mathbb{R} $$
[Game Theory Article](https://www.sciencedirect.com/science/article/pii/B9780128044520000063)









