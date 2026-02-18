## Limit Points and Closure
- **Definitions**
	- Let $A$ be a subset of a topological space. a point $x\in X$ is said to be a **limit point** of **A** if every open set, U, containing x contains a point of $A$ different from $x$.
	- Let $A$ be a subset of a topological space. Then the set $A \cup A'$ consisting of $A$ and all its limit points is called the **closure of $A$** and is denoted by $\bar{A}$
	- Let $A$ be a subset of a topological space. Then $A$ is said to be **dense** in $X$ or **everywhere dense** in $X$ if $\bar{A} = X$.

- **Propositions**
	- Let $A$ be a subset of a topological space. Then $A$ is closed if $(X, \mathcal{T})$ if and only if $A$ contains all of its limit points.
	- Let $A$ be a subset of a topological space and $A'$ the set of all limit points of $A$. Then $A \cup A'$ is a closed set.
	- Let $A$ be a subset of a topological space. Then $A$ is dense in $X$ if and only if every non-empty open subset of $X$ intersects $A$ non-trivially.

## Neighbourhoods
- **Definitions**
	Let $N$ be a subset of $X$ and $p$ a point in $N$. Then $N$ is said to be a **neighbourhood** of the point $p$ if there exists an open set $U$ such that $p\in U \subseteq N$ 

- **propositions**
	Let $A$ be a subset of a topological space. A point $x \in X$ is a limit point of $A$ different from $x$.

- **corollaries**
	- Let A be a subset of topological space. Then the set $A$ is closed if and only if $\forall x \in X\setminus A$ there is a neighbourhood $N$ of $x$ such that $N \subseteq X \setminus A$. 
	- Let $U$ be a subset of a topological space. Then $U \in \mathcal{T}$ if and only if $\forall x \in U, \exists N(x) \text{ s.t } N\subseteq U$. ($N(x)$ is the neighbourhood $N$ of $x$)
	- Let $U$ be a subset of a topological space. Then $U \in  \mathcal{T} \text{ iff } \forall x \in U \exists V \in \mathcal{T} \text{ s.t } x \in V \subseteq U$.

## Connectedness 
- **Definitions**
	a topological space is said to be **connected** if the only clopen subset of $X$ are $X$ and $\emptyset$.

- **Propositions**
	- Let $T$ be a clopen subset of $\mathbb{R}$. Then either $T= \mathbb{R}$ or $T = \emptyset$.
	- The topological space $\mathbb{R}$ is connected.

- **Lemma**
	Let $S$ be a subset of $\mathbb{R}$ which is bounded above and let $p$ be the supremum of $S$. If $S$ is a closed subset of $\mathbb{R}$, then $p \in S$. 