Generating Meaning. 

[1] Definition of meaning as embodied interaction with the world. 
[2] Extension of this through example of language-games. Meaning derived from use and the subsequent homonymous character of words. 

[3] The existence of certain non-linguistic forms of life. 
[D. 3a] The ability for these non-linguistic forms of life being captured. 
[3a] Wittgenstein and Saussure on Grammar and structures of language. 

"Grammar describes the use of words in the language. So it has somewhat the same relation to the language as the description of a game, the rules of a game, have to the game." (PG:60)

Unsure how to include the following: 
	Furthermore, “It is grammatical rules that determine meaning (constitute it)” (PG:184).

[3B] Can we record these structures 
"Of course a man will often say. to himself while watching "oh, so that's the rule"; and he might perhaps write down the rules as he observes them" (PG:62)

[4] Umiak and Octopus test showing that we require non-linguistic forms of interaction to make sense of meaning. 

[5] Markov text generators. Text generation cannot be purely probabilistic. It needs to capture these non-embodied features found in (previous discussion of Wittgenstein and Saussure)

___

Artificial Language

[1] Discussion of John Peters Versifying Tables. 

In this way, what came before determines the permissibility of what comes after. 
“Whether a proposition entails another proposition must be clear from the grammar of the proposition and from that alone. (PG: 256).

Poetry as a type of language-game. (Stress-> Unstress)


[2] John Clark and the "Eureka"

[3] The machine took in an algorithm which expressed a certain structure of language, and then reproduced it mechanically. 

___

Neural Networks & LLM

[1] History of the Neural Network as replicating the vision of a Frog's eye. 

[2] Patterns are encoded spatially. Even from the beginning of NN research. 

[3] LLMs as a type of NN which finds patterns in text in certain ways (I.e., how do they encode grammar?)

[D. 3] Given their massive success, currently existing linguistic theories have hard a hard time explaining their success. Chomskyan linguistics for example would require the LLM to have [...], the same structures which are inherent in humans. Instead it is our previous exposition of Wittgenstein and Saussure which best explain their functioning 

[4] Discussion of how they encode grammar 

Every significant word or symbol must essentially belong to a “system,” and . . . the
meaning of a word is its “place” in a “grammatical system.” Wittgenstein, Philosophical Occasions, 51

meaning of a word is its “place” in a “grammatical system.” Wittgenstein, Philosophical Occasions, 51

Context Correlates: 
in ordinary grammar one might as well distinguish "shape words", "colour words", "sound words", "substance words" and so on as different parts of speech.' (PG:61) 

"a linguistic unit may be compared to a single part of a building e.g. a column. A column is related in a certain way to architrave it supports. This disposition, involving two units co-present in space, is comparable to a syntagmatic relation. On the other hand, if the column is Doric, it will evoke mental comparison with the other architectural orders (Ionic, Corinthian, etc.), which are not in this instance spatially co-present. This relation is associative." (CLG: 171)


[D. 4] Need to expand on this discussion and fill in with Wittgenstein quotes. 

___

Chess. 

[1] What does separation between langue and parole entail? 
What does the LLM Lose: “Just as it is impossible to take a pair of scissors and cut one side of paper without at the same time cutting the other, so it is impossible in a language to separate sound from thought, or thought from sound. To separate the two for theoretical purposes takes us into either pure psychology of pure phonetics, not linguistics.” (CLG: 157)
	The sign cannot be entirely divorced from the element of speech. 

One is inclined to make a distinction between rules of grammar that set up "a connection between language and reality" and those that do not. A rule of the first kind is "this colour is called 'red' ", - a rule of the second kind is "-- p = p". With regard to this distinction there is a common error; language is not something that is first given a structure and then fitted on to reality. (PG:89)

They only capture semantic regularities, parts of the language game as the words relate to each other. Which allows them to separate the occurrence of certain language games, but this is not an entirety.

[2] Why can we understand them? 
The reason we are able to understand LLMs is because we treat their works with charity. Keep some of the Ern Malley Discussion. 

However, because these LLMs only have access to langue, they are unable to perform certain activities which require both. 

[3a] Why are they able to play basic chess. 
They are able to play basic chess because they “marinating in Big Data” to use Chomsky’s terminology (Circling the void paper for citation)

They cannot perform tasks in which linguistic references are a necessary part of the activity, in which the signs cannot be structurally extricated from the world. 

[3] What are they missing? 
However, they cannot capture the ostensive meanings between signs that lay in embodied experience. Such as the rules of chess. the LLM captures the semantic regularity of algebraic notation (a type of way to denote chess moves) and their correspondence with each other, but it is not able to capture the actual rules of chess. In comparison, a machine learning model trained to play chess has these rules built in to its programming.  
  
There are different dimensions to language games, and semantic regularity is only one of them, ‘When one shews someone the king and says: 'This is the king', this does not tell him the use of this piece--unless he already knows the rules of the game up to this last point’. Philosophical Investigations, section 31. 

The occurrence of certain moves in chess that are illogical for us are perfectly possible for a large language model. Its training data will bias the relationship between the previous move and the current one in order to produce an output. For us, it’s obvious that a pawn cannot move three spaces ahead, however, this does not mean that a pawn is unable to occupy the square three spaces ahead in the span of a game.

Playing as white, the move Pawn from E2 to E3 or E4 are perfectly permissible, however, Pawn from E2 to E5 is not. Still, it’s possible for a pawn to move to E5 (given that it was placed on E4). The problem for the LLM is that the current board state is not tracked, only the semantic similarity between different occurrences of moves, and given a move from black (such as Knight to D4) whose closest semantic relative is E5, the LLM will play E5 regardless of if this is a legal move or not.

Other games, such as that of Go, or XiangQi also prove challenging for LLMs. 



