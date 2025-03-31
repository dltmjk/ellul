## Five Modes of Forming [[Constructions]]
1. Variables are *simple* constructions 
2. All other constructions have constituent parts 
	1. In defining other classes of constructions, we need to specify the *modes* of forming constructions 

### Trivialization 
1. if $X$ is an entity. The trivial construction that can be made is $X$ itself, symbolized as $^0X$
	1. If $X$ is a construction which produces numbers for any $v$ (This is called a $v$-construct, e.g. $X$ $v$-constructs a number) then $^0X$ will still $v$-construct $X$. Therefore, whatever is $v$-constructed for $^0X$ does not depend on $v$
	2. $^0X$ is a construction, whereas $X$ is any entity whatsoever. 

### Execution 
1. if $X$ is a construction then $^1X$ is $X$ 
	1. This is the construction that consists in carrying out construction $X$ must be $X$ 
	2. If $X$ is not a construction then $^1X$ will yield nothing because a non-construction cannot be carried out. 
		1. This can be extended to $v$-improper constructions. 
		2. Therefore if $X$ is a $v$-improper construction or not a construction then $^1X$ is $v$-improper.

### Double Execution 
1. If the construction of X is also a construction then we can also execute the result. 
	1. $X \longrightarrow ^2X \longrightarrow$  
	2. Same rules apply, if $X$ is $v$-improper\not a construction then $^2X$ is also $v$-improper
		1. Furthermore, if $X$ $v$-constructs something that isn't a construction or a $v$-improper construction then $^2X$ is not a construction/$v$-improper
	3. Otherwise, if all necessary criteria is met, then $^2X$ $v$-constructs the output of $v$-constructing $X$

### Composition 
1. "Let $F$ be a construction of a mapping and $X$ a construction of an argument of the mapping. $F$ and $X$ can be combined into a compound construction which consists in executing $F$, thus obtaining a mapping, then executing $X$, thus obtaining an argument of the mapping, and then applying the mapping to the argument, thus obtaining the value (if any) of the former at the latter. We shall call this compound construction the 'composition' of $F$ and $X$, or briefly, $[FX]$. (Note that the compound symbol '$[FX]$' names the construction, not the number constructed by it.)" 
	1. The composition $[X_{0}X_{1} \dots X_{m}]$ consists in executing $X_{0}$ to obtain a mapping and then executing $X_{1}$ and $X_{m}$ to get $m$ entities and applying that mapping to the $m$-tuples you just generated.   

### Closure
1. When you are presented with an incomplete construction
2. Revisit This

## Ramified Hierarchy
1. The hierarchy theory is based on [[Variables]] and the way to form constructions described above. 
2. The objects we are working with may be classified into several different categories. 
	1. We start by defining *first-order* types. Types without entities or constructions 
	2. *second-order types* are types which comprise objects containing variables ranging over first-order types and constructions involving such variables 
	3. *third-order types* are types which are objects containing variables that range over first and second order types. 

## Definition 16.1 
1. Arithmetic is concerned with two collections which form a base. Infinite collection $\alpha$ of $\mathbb{N}$ and a collection, $o$ of two truth values $T$ and $F$ 
	1. The typological classification of objects that are present within arithmetic. 
		1. e.g. $\alpha$ represents a number, 1 or 0 
		2. $\text{Suc}$ - $(\alpha \alpha)$ - successor mapping 1 to 2, 0 to 1. 
		3. $\text{Odd}$ that takes in a number a number and returns the truth value of whether it is odd or not - $(o \alpha)$ 