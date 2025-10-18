This section begins by establishing a working definition of opacity before outlining its three main types: social, technical, and systematic. The discussion then turns primarily to systematic opacity and how its intensity can vary relative to an agent. Next, we examine the formulations of opacity proposed by Zerilli, Creel, and Lipton, showing that their key differences lie in what each considers epistemically relevant. Finally, we argue that when an agent can justifiably abstract certain parts of a system, they can thereby reduce its overall opacity.

While many definitions of epistemic opacity have been given over the years with some consensus, the earliest and most popular one is Humphreys:

“A process is epistemically opaque relative to a cognitive agent X at time t just in case X does not know at t all of the epistemically relevant elements of the process. A process is essentially epistemically opaque to X if and only if it is impossible, given the nature of X, for X to know all of the epistemically relevant elements of the process” (2009, pg. 617)

This definition of opacity asserts that a lack of knowledge of epistemically relevant elements is sufficient for a process P to be opaque. It’s important to note that opacity is always in reference to a human agent. Humphreys (2009, pg. 617) characterises this opacity problem as how “humans can understand and evaluate computationally based scientific methods that transcend [their] own abilities”. Therefore, a system can be opaque to one agent and not to another if they differ in ability. 

However, this seems to present certain problems when viewed in relation to most scientific instruments. As Louis Bucciarelli (1994, Thing Knowledge pg.13) points out “Do you know how your telephone works?” (p.3, Designing Engineers). He explains that while one scientist might be able to parse one particular aspect of a telephone's functioning (for example, how sound is produced by an electric current), they might not be able to review the exact functioning of the algorithms employed in noise suppression (Cite Baird). Either because these algorithms are hidden from public view or because they lack the technical know-how. Either way, they are unable to fully ensure that the telephone is functioning as intended. This presents a general problem for most scientific discovery because every scientist utilises tools that they are unfamiliar with. For example, a biologist in the process of recording their results from an experiment may use the data analytics tools of a spreadsheeting program that is technically opaque to them. The reliability of their experimental results seem to epistemically depend on the reliability of the spreadsheeting program. If the scientist is unable to justify both parts, does this make the former results unreliable? 

Obviously not. Given the varied and distributed nature of scientific research, a great deal of trust is required, since it’s impossible for any individual to double-check and fully understand all the prior information and tools they rely on. Research, especially those of large groups, produces work where no single agent can interpret each moving part. Hardwig (1985, Koskinen) states that in cases like this — of collective knowledge production — trust must stand in for justification. Granted that this trust is regulated in a few ways (Frost-Arnold 2013). Some informal, for instance the belief that your scientific peers are acting honestly, and some regulated, such systems of peer-review. These procedures of epistemic checking, when followed correctly, reduce error and the role of trust within knowledge production (Wilholt, 2013).

Koskinen argues that in cases of scientific instruments, trust is warranted as long as there is an agent who “understands how the instruments work, takes responsibility [for] them in an epistemically acceptable manner, and can be trusted” (Koskinen pg. 7). Returning to our example of the biologist, we can justify their usage of technically opaque instruments as long as there is an agent, such as the manufacturer, that can take responsibility. Results from large-scale scientific endeavours, such as the LHC, are justified on the basis that every part has an agent for which it is not epistemically opaque.

___
DNNs are often said to be opaque for every possible agent (Cite Burell). This differs from our previous conception of opacity as being agent specific. If we accept that DNNs are opaque in this manner, then there is a type of opaqueness that arises out of a systems construction. Following from this, we can identify three types of opacity: systematic, technical, and social ([[Sources of Opacity in Computer Systems; Towards a Comprehensive Taxonomy]]). Alvarado (CITE) gives his formulation of social opacity: 

"Division of labor, proprietary limitations on access, intentional secrecy, etc. all contribute to making the workings of a system, process or device inaccessible to some while accessible to others, and hence generally, and relatively epistemically opaque as defined above." pg. 4 [[Alvarado Epistemic Opacity Types]]

Social opacity concerns the agent, their position, and their abilities, but it can be alleviated through epistemic interdependence. By contrast, systematic opacity arises from the structure of the system. Despite appearances, this type of opacity is still agent-specific; however, unlike technical opacity, it pertains to certain properties of the system that limit the agent’s understanding, rather than to qualities of the agent.

Therefore, there must be some condition, or property, that when applied to a system, renders it epistemically opaque (San Pedro degrees of epistemic 2020). For example, we previously saw how social factors prevented an agent from familiarising themselves with a system. If we continue with this logic, we can say that there are certain properties χ that induce opaqueness within a model, i.e. property χ when applied to a model prevents an agent’s awareness of the epistemically relevant parts. Consequently, we can claim that the lack, or toning down, of this property increases the transparency of a system. 

Opacity is often treated as a binary property. For example, Søgaard argues, “If both ϕ and ψ are properties of a DNN δ and sources of opacity, removing ϕ is insufficient to make δ transparent” (p. 226). In this view, a system either is opaque or it is not, with no in-between. However, there are problems with this conception. If opacity is always relative to an agent, it is entirely possible for a system to be opaque to an agent at time t, but for that opacity to decrease at a later time t₁ if the agent improves their knowledge in the interim (Saam, 2018). While this approach may not make the DNN fully transparent, it would increase the overall level of transparency within the system. Accordingly, we can also say that if a system possesses a given property, reducing or removing that property decreases its opacity. Furthermore, different forms of opaqueness produce different kinds of opacity. Returning to the previous example, it seems we are dealing with both size-opaqueness and dimensionality-opaqueness, each of which affects the agent and the system’s overall opacity in different ways.

It has become more common to speak of ‘degrees of epistemic opacity’ (Duran and Formanek 2018, Lenhard 2018, San Pedro 2020). The importance of establishing this is that, once a certain gradation of opacity has been established, we can implement methods to reduce the effect of an opaque property on a model. To accomplish this, we must also break down the different types of opaqueness. It seems that the type of opaqueness produced by social factors differ from the type produced by the size of a system. Size is a property that induces technical opacity and prevents an agent from evaluating all the epistemically relevant parts. Different formulations of opacity classify it based on what is considered epistemically relevant. For example, Zerilli argues for model opacity along the lines of linearity and dimensionality. A linear system with fewer dimensions is more fathomable than an alternate higher dimensional system. In which fathomability concerns a human observer who, in the former low-dimensional case, is able to “contemplate the entire model at once” (Lipton 2017, 4) (Zerelli, 7). An unfathomable system, for example, would be an extremely large computer simulation model with billions of parts. In this case, size, in the form of dimensions, is our $\chi$ will induce opaqueness and epistemic relevancy is every single operation the system performs. 

However, as long as this simulation maintains linearity, it retains another two of Zerilli’s properties: intelligibility and tractability. Tractability is whether a model can be run on a machine whereas intelligibility is if the relationship between a model’s subparts can be determined, despite size. Therefore, a large and complex model remains intelligible if an agent can trace the nature and relationship of the model’s constituent parts. For example, a computer program which multiplies large numbers may be opaque due to its un-fathomability given that a human agent cannot possibly hope to work through each binary operation the program performs. However, it still maintains the properties of tractability and intelligibility since the agent can abstract parts of the program to see how they causally relate to another. 

Both Creel (CITE) and Lipston (CITE) have raised distinctions along similar lines. However, instead of centring discussion around opacity, they evaluate a system in regards to three criteria of transparency. “Run” transparency, the first category, is the easiest to fulfil and requires the ability to survey the implementation code along with input data. The latter two categories – algorithmic and structural transparency \footnote{The opposite being algorithmic and structural opacity} – both pose problems for DNNs. Algorithmic transparency requires an agent to be aware of the high-level logical rules (which functions) the model uses in the transformation of input to output. Whereas structural transparency requires an agent to understand how the architecture of a system encodes a specific function. 

Zerilli’s fathomability and Creel’s run transparency both establish opacity by arguing that no human agent could familiarise themselves with each step. Within these classifications, the epistemically relevant parts of the program are each operation the computer performs at a hardware level. However, if this is the case then every computer program must be necessarily opaque and therefore unreliable? For example, a simple program which takes the input of two numbers and returns their sum – if run on a modern operating system – will require billions of operations. Is this program opaque? According to Creel, it exhibits run opacity but not algorithmic opacity, because the high-level logical rules governing the program are accessible. An agent inspecting the program can abstract portions of the system into higher-level concepts. With sufficient knowledge of computer internals and assembly language, the agent can justify causal reasoning about the program’s behaviour, such as linking specific lines of code to underlying logic gates or transistor operations. Given enough time, it would even be theoretically possible to examine each binary operation and fully justify the program’s functioning—for example, identifying that one clump of transistors encodes the character ‘h’ and interacts with another clump to produce ‘i,’ thereby outputting ‘hi.’

Within each formulation, opacity refers to a lack of understanding of the epistemically relevant parts, where the definition of what counts as epistemically relevant varies depending on the type of opacity being considered. Relevancy ranges from familiarity with the underlying technical components (in the form of transistors or other sorts of hardware) to an understanding of the higher-level rules. 

If an agent is unable to abstract or explain how a system organizes low-level operations into higher-level rules, the system is considered algorithmically or structurally opaque. These forms of opacity are generally more significant than run opacity, as they prevent the agent from understanding the system’s underlying logic or architecture, even if the program can be executed. The epistemic problem posed by algorithmic opacity, compared to run opacity, was first highlighted in a 1966 Scientific American article by Anthony Oettinger, who argued that the most important type of understanding is being functionally (i.e., conceptually) aware of how it mimics an input-output relation. Furthermore, a researcher is justified in being unaware of lower-level constituents if they can explain how these constituents are abstracted into a higher-level function.

This ties directly back to our discussion of degrees of opacity. If an agent is able to abstract certain parts of a system and make them easily graspable, they reduce the system’s overall opacity. An agent who can provide reasons for the functioning of specific subsets of a system, even without being fully aware of every part, similarly reduces the system’s opacity. If algorithmic opacity arises from an agent’s lack of knowledge of higher-level rules, then constructing such rules for a system’s functioning allows the agent to decrease its overall opacity.

Therefore, if an agent understands, or is able to justifiably show, how a certain function emerges from its component parts, they can justify their reliance without being familiar with every operation. Given this, we can model opacity, and understanding, as a type of scale. At the bottom is run-transparency, or opacity that is caused by a lack of understanding of the lowest level components. Within the context of DNNs, these are the transistors used to calculate weights and biases. Abstracted from this is the actual programming implementation of the neural network, and at the highest end is conceptual understanding of the model's internal dynamics. 

To recap, opacity is an agent-relative condition that manifests from the existence or abundance of a certain property $\chi$ within a system. There are different taxonomies of opacity, depending on what we consider to be epistemically relevant — ranging from each operation to an algorithmic understanding. Opacity presents problems with reliability insofar as an agent is unable to give reasons for why a certain result is given from some inputs. In essence, within all these different types of opacity, what remains constant is that an agent is not able to understand the result by reference to whatever is considered an epistemically relevant element. 

An instrument is only considered reliable if an agent can take responsibility for it. This means that an agent must also be able to *explain* the result to another agent in reference to an epistemically relevant element. We can only place our trust in an agent if they are able to freely share information that would make an instrument transparent. This type of epistemic demand on an agent is broadly in line with conceptions of understanding. Petri Ylikoski (CITE) gives his account of evaluating understanding: 

> When we evaluate somebody’s understanding, we are not making guesses about his or her internal representations, but about the person’s ability to perform according to set standards. The concept of understanding allows that the ability can be grounded in various alternative ways, as long as the performance is correct. Furthermore, the correctness of the internal model is judged by the external displays of understanding, not the other way around. This makes understanding a behavioral concept (Ylikoski, 2009, p. 102, duran understanding w/ toy models).

___
From here, we will evaluate the training stage of the DNN and the deployment DNN separately to see whether opacity presents problems and, if so, at what point these arise. We argue that opacity presents few epistemic problems in justifying the reliability of a T-DNN if we treat it as a causal instrument. However, opacity presents significant problems for the deployment DNN due to its status as a model instrument. 

The justifications differ for the T-DNN and the deployment DNN because they are different types of instruments with different functions. A causal instrument needs to pick up on a certain causal relationship, whereas the model instrument needs to represent this relationship. Therefore, when justifying the results of the training stage of a DNN, we don't need to appeal to anything except the underlying architecture because the utility of the instrument is to pick up on a function. While it might be algorithmically opaque, reliability can be justified on the basis of structural transparency. 

On the other hand, a model instrument needs to represent a function in a semantically intelligible way in order for an agent to justify the output. These instruments require a structure which is explanatory with regards to its causal decision making and the relationship with an underlying phenomenon. Therefore, an agent requires access to the relevant higher-level rules to justify this bidirectional relationship. 






It seems that opacity is if an agent is unable to give reasons, either technical or conceptual, for why a system produces a certain output. This causes problems for reliability because the agent these reasons strengthen 

Therefore, for an instrument to be justified there must be an agent who can give reasons for its producing an output. 

We provide a reformulation of opacity in the form of explanation within the philosophy of science. 

Explanations 



There is a way in which DNNs are fully transparent because an agent can inspect every parameter of the system. Algorithmic opacity is induced because of certain properties that prevent an agent from understanding what parameters encode which functions, therefore preventing understanding of the high-level rules the model uses.  












What we require is a type of semantic explanation for the functioning of a system. 


With all this established, we need to ask how opacity presents a problem for the DNN. 



###     START with  filling in the Creel stuff

What really is opacity - Creel 

Prevents the giving of explanation of a system. Which is true for models, but not for causal instruments. 

Opacity prevents a certain type of explanation 

However, opacity only presents problems with a system when a system is expected to behave like a model. A causal instrument only requires that it performs the same generic function consistently. Which DNNs have been proven to do. 

Extend main arguments
1. Justifying the DNNs can be broken down into two instruments 
2. That causal instruments do not require explanation that is impeded by opacity 


Opacity concerns the lack of having an explanation for the reasons to trust a system, given the specific functioning of a system. 







===Kind of useless=== 









