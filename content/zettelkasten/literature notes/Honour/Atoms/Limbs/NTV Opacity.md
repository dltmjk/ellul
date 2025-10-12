While many definitions of epistemic opacity have been given over the years with some consensus, the earliest and most popular one is Humphrey’s

“Here a process is epistemically opaque relative to a cognitive agent X at time t just in case X does not know at t all of the epistemically relevant elements of the process. A process is essentially epistemically opaque to X if and only if it is impossible, given the nature of X, for X to know all of the epistemically relevant elements of the process” (CITE HUMPHREY)

This definition of opacity asserts that a lack of knowledge of epistemically relevant elements is sufficient for a process P to be opaque. It’s important to note that opacity, despite manifesting out of certain properties of a system, is always in reference to a human agent. Humphrey (2009, pg. 617) characterises this opacity problem as a how “humans, can understand and evaluate computationally based scientific methods that transcend our own abilities”. We can see that the knowledge of an agent X plays an important role in whether a system is opaque or not. Therefore, a system can be opaque to one agent and not to another because a lack of knowledge of epistemically relevant elements is sufficient for a process P to be opaque. 

However, this seems to present certain problems when viewed in relation to most scientific instruments. As Louis Bucciarelli (1994, Thing Knowledge pg.13) points out “Do you know how your telephone works?” (p.3, Designing Engineers). He explains that while one scientist might be able to explain one particular aspect of a telephones functioning (for example, how sound is produced by an electric current), they might not be able to parse the exact functioning of the algorithms employed in noise suppression (Cite Baird). Therefore, they are unable to fully ensure that the telephone is functioning as intended due to a lack of technical know-how, preventing transparency. This presents a general problem for most scientific discovery because every scientist utilises tools that they are unfamiliar with. For example, a biologist in the process of recording their results may use the data analytics tools of a spread-sheeting program that is technically opaque to them. Does this mean that scientists are unable to justify the usage of certain instruments that they employ?

Given the varied and distributed system of scientific research, large elements of trust are required since it’s impossible for an individual to double check and fully understand all the previous information they relies on. Research, especially those of large groups, produce work in which no singular agent can interpret each moving part. Hardwig (1985, Koskinen) states that in cases like this – of collective knowledge production - trust stands in for justification. Granted that this trust is regulated in a few ways (Frost-Arnold 2013). Some informal, for instance the belief that your scientific peers are acting honestly, and some regulated, such systems of peer-review. These procedures of epistemic checking, when followed correctly, reduce error and the role of trust within knowledge production (Wilholt, 2013).

As established before, instruments cannot be trusted - they can only be relied on. Therefore, in cases of scientific instruments, trust is warranted as long as there is an agent who “understands how the instruments work, takes responsibility of them in an epistemically acceptable manner, and can be trusted” (Koskinen pg. 7). Returning to our example of the biologist, we can justify their usage of technically opaque instruments as long as there is an agent, such as the manufacturer, that exists and can take responsibility. Results from large-scale scientific endeavours, such as the LHC, are justified on the basis that every part has an agent for which it is not epistemically opaque.

___
Therefore, there are certain types and levels of opaqueness which are produced by certain properties. Types of opacity explored in our previous examples seem to stem from a social nature. Generally, we can classify opacity in three types: systematic, technical, and social ([[Sources of Opacity in Computer Systems; Towards a Comprehensive Taxonomy]]). Both technical and social sources were covered briefly and concern an agent’s technical know-how and their resources. Alvarado (CITE) gives his formulation of social opacity: 

"Division of labor, proprietary limitations on access, intentional secrecy, etc. all contribute to making the workings of a system, process or device inaccessible to some while accessible to others, and hence generally, and relatively epistemically opaque as defined above." pg. 4 [[Alvarado Epistemic Opacity Types]]

However, these types of opacity are inevitable and are alleviated by a level of epistemic inter-dependence. Social opacity concerns the agent and their position and ability. In comparison, systematic opacity concerns the system and prevents an agent from knowing all epistemically relevant parts through no fault of the agent. 

Therefore, there must be some condition, or property, that when applied to a system, renders it epistemically opaque in a certain way (San Pedro degrees of epistemic 2020). For example, in our previous section we saw how social factors prevented an agent from familiarising themselves with the parts of a system. If we continue with this logic, we can say that there are certain properties χ that induce opaqueness within a model, i.e. property χ when applied to a model prevent an agent from awareness of the epistemically relevant parts. Furthermore, the lack, or toning down, of this property increases the transparency of a system. 

Most literature on opacity treats it as a binary property. For example, they would argue that if more than two χ properties are present, the lowering of one doesn’t change the opaqueness of a system. If we imagine a system that is opaque because of its dimensionality, modifying the size should not make a difference to the overall opaqueness. So, a system either is, or is not opaque without any in-between. However, if opacity is in respects to an agent understanding, then it seems fair to model it as a type of scale because if a model can have varying levels of opaqueness towards two different agents, then it is feasible to speak of a gradient of opaqueness. For example, it is fully possible for a system to be opaque to an agent at time t but to reduce that opacity at time t1 if an agent improves their knowledge in-between (Saam 2018). Therefore, we can also say that if a system has property $\chi$ then by lowering, or removing $\chi$, it reduces its opacity. Furthermore, different types of opaqueness produce different types of opacity. If we return to previous example – it seems we are dealing with both size-opaqueness and dimensionality-opaqueness.

Some attempts have been made to speak of ‘degrees of epistemic opacity’ (Duran and Formanek 2018, Lenhard 2018, San Pedro 2020). The importance of this is that, once a certain gradation of opacity has been established, we can implement methods to reduce the effect of an opaque property on a model. To accomplish this, we must also break down the different types of opaqueness. It seems that the type of opaqueness produced by social factors (such propriety limitations) differ from the type produced by the size of a system. This sort of technical opacity stops an agent from evaluating all the epistemically relevant parts. Different taxonomies of opaqueness give different types of opaqueness depending on what one considers epistemically relevant. For example, Zerilli argues for model opacity along the lines of linearity and dimensionality. A linear system with fewer dimensions is more fathomable than an alternate higher dimensional system. In which fathomability concerns a human observer who, in the former low-dimensional case, is able to “contemplate the entire model at once” (Lipton 2017, 4) (Zerelli, 7). An unfathomable system, for example, would be an extremely large computer simulation model with billions of parts. In this case, size in the form of dimensions, is our $\chi$ will induces opaqueness and epistemic relevancy is every single operation the system performs. 

However, as long as this simulation maintains linearity, it retains another two of Zerelli’s properties - intelligibility and tractability. Tractability is whether a model can be run on a machine whereas intelligibility is if the relationship between a model’s subparts can be determined, despite size. Therefore, a large and complex model remains intelligible if an agent can trace the nature and relationship of the model’s constituent parts. For example, a computer program which multiplies large numbers may be opaque due to its un-fathomability given that a human agent cannot possibly hope to work through each binary operation the program performs. However, it still maintains the properties of tractability and intelligibility since the agent can abstract parts of the program to see how they causally relate to another. 

Both Creel (CITE) and Lipston (CITE) have raised distinctions along similar lines. However, instead of centring discussion around opacity, they evaluate a system in regards to three criteria of transparency. “Run” transparency, the first category, is the easiest to fulfil and requires the ability to survey the implementation code along with input data. The latter two categories – algorithmic and structural transparency – both pose problems for DNNs. Algorithmic transparency requires an agent to be aware of the high-level logical rules (which function) the model uses in the transformation of input to output whereas structural transparency requires an agent to understand how the architecture of a system encodes a specific function. 

Zerelli’s fathomability and Creel’s run transparency both establish opacity by arguing that no human agent could familiarise themselves with each step. Within these classifications, the epistemically relevant parts of the program is each operation the computer performs at a hardware level. However, if this is the case then every computer program must be necessarily opaque and therefore un-reliable? For example, a simple program which takes the input of two numbers and returns their sum – if run on a modern operating system – will require billion of operations. Is this program opaque? According to Creel, it is run-opaque, but not algorithmically opaque because we are privy to the higher-level logical rules. An agent, when inspecting this program, has good reasons for abstracting certain parts of the system into concepts. An adequate knowledge of computer internals and assembly language allows them to justify a chain of causal reasoning regarding the program. They can claim that a certain line of code corresponds to a clump of transistors firing, justifying their reasoning through their knowledge of logic gates. If needed and given enough time, they could theoretically work through each binary operation to secure justification. Given that they can give good reasons for abstracting a certain set of operations into a certain function. E.g. this clump of transistors is responsible for encoding the character 'h' and interact with another clump which produces 'i' to output 'hi'.

Within each system, opacity is the lack of understanding of the epistemically relevant parts. Where what counts as an epistemically relevant part changes depending on the type of opacity you are trying to combat. Opacity ranges from familiarity of the underlying technical components (in the form of transistors or other sorts of hardware) to an understanding of the higher-level rules. Being unable to understand the structural and relational parts of each of these components means that an agent would, potentially, be unaware of how an output was reached from input. 

If an agent understands how a certain functions emerge from certain other parts in a system. They can justify their reliance without being familiar with every operation. Furthermore, we can model opacity as a type of scale. At the bottom is run-transparency, or opacity that is caused by a lack of understanding of the lowest level components. Within the context of DNNs, these are the transistors used to calculating weights and biases. From there, is the actual programming implementation of the neural network, and at the highest end is conceptual understanding of the models internal dynamics. 

To recap. Opacity is an agent-relative condition that manifests from the existence or abundance of a certain property $\chi$ within a system. There are different taxonomies of opacity, depending on what we consider to be epistemically relevant - ranging from each operation to an algorithmic understanding. Opacity presents problems with reliability insofar as an agent in unable to give reasons for why a certain result is given from some inputs. In essence, within all these different types of opacity, what remains constant is that an agent is not able to understand the result by reference to whatever is considered an epistemically relevant element. 

As an instrument is only considered reliable if an agent can take responsibility. This means that an agent must also be able to *explain* the result to another agent in reference to an epistemically relevant element. We can only place our trust in an agent if they are able to freely share information that would make a instrument transparent. 

This type of epistemic demand on an agent is broadly in line with conceptions of understanding. Petri Ylikoski (CITE) gives his account of evaluating understanding: 

> When we evaluate somebody’s understanding, we are not making guesses about his or her internal representations, but about the person’s ability to perform according to set standards. The concept of understanding allows that the ability can be grounded in various alternative ways, as long as the performance is correct. Furthermore, the correctness of the internal model is judged by the external displays of understanding, not the other way around. This makes understanding a behavioral concept (Ylikoski, 2009, p. 102, duran understanding w/ toy models).

If understanding is relative to the epistemically relevant element, then explanation will also depend on it. Furthermore, the type of explanation will change depending on the type of instrument they are justifying. Within the philosophy of science there are multiple forms of explanation. 

We will argue that we require a causal account linking input and output. 

For the T-DNN, our form of explanation can appeal to the type of input data in justifying why it reached a certain function. 

Whereas for deployment, models require an agent to know how their link the world in order for any explanation to take place. Therefore opacity presents problems


___
From here, we will evaluate the training stage of the DNN and deployment DNN separately to see if opacity presents problems and, if they do, at what point this starts. We argue that opacity presents no epistemic problems in justifying the reliability of a T-DNN if we treat it as a causal instrument. However, opacity presents significant problems for the deployment DNN due to its status as a model instrument. 

The justifications differ for the T-DNN and the deployment DNN because they are different types of instruments with different functions. A causal instrument needs to pick up on a certain causal relationship, whereas the model instrument needs to represent this relationship. Therefore, when justifying the results of the training stage of a DNN, we don't need to appeal to anything except the underlying architecture because the function of the instrument is to pick up on a function. While it might be algorithmically opaque, reliability only requires run-transparency. 

On the other hand, a model instrument needs to represent a function in a semantically intelligible way in order for an agent to justify the output. These instruments require a structure which is explanatory in regards to its causal decision making and the relationship with an underlying phenomenon. Therefore, an agent requires access to the higher-level logical rules to justify this bidirectional relationship. 







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









