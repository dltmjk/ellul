\noindent A problem with Jeffreys conditionalizatin and other relevant interpretations can be sketched as follows. We will reconstruct the argument Rescorla (2020) puts forward in \cite{rescorla2022improved}. Consider three mutually exclusive propositions $E_1, E_2, E_3$, initially assigned probabilities: \\

$P_{\text{old}}(E_1) = \frac{1}{4}$, \quad $P_{\text{old}}(E_2) = \frac{1}{4}$, \quad $P_{\text{old}}(E_3) = \frac{1}{2}$. \\

\noindent A further proposition $A$ has conditional probabilities: \\

$P_{\text{old}}(A \mid E_1) = 0$, \quad $P_{\text{old}}(A \mid E_2) = \frac{1}{2}$, \quad $P_{\text{old}}(A \mid E_3) = 0$. \\
  
\noindent  Thus initially:
  \[
  P_{\text{old}}(A \mid E_1 \lor E_2) = \frac{1}{4}
  \] \\

\noindent You then gain some evidence strongly favoring $E_2$, yet not completely ruling out $E_1$. Thus, your updated probabilities might become: $P_{\text{new}}(E_1) = \frac{1}{100}$, \quad $P_{\text{new}}(E_2) = \frac{99}{100}$, \quad $P_{\text{new}}(E_3) = 0$.
Now you are fully certain that $E_1 \lor E_2$ is true (probability = 1), but internally, probability mass has shifted dramatically towards $E_2$. If we follow the problematic formulation above, we would conditionalize on $E_1 \lor E_2$: 
\[
P_{\text{new}}(A) = P_{\text{old}}(A \mid E_1 \lor E_2) = \frac{1}{4}
\]

\noindent  However, intuitively, this seems wrong, because the probability mass shifted heavily toward $E_2$, suggesting that $P_{\text{new}}(A)$ should actually be closer to $P_{\text{old}}(A \mid E_2)$ (i.e., $\frac{1}{2}$), since $E_2$ now dominates your probability space. Therefore, the problematic formulation fails to handle these kinds of \emph{Jeffrey-style shifts}. \cite{rescorla2022improved} \\



