## Topology
- **Definitions** 
	- Let $X$ be a non empty set. A set $\mathcal{T}$ of subsets of $X$ is said to be a **topology** on $X$ if :
		- $\{X , \emptyset \} \subseteq \mathcal{T}$
		- $\bigcup_{i \in I} U_i \in \mathcal{T} \text{ for any } \{U_i\}_{i \in I}  \subseteq \mathcal{T} \text{ such that } I \subseteq \mathbb{N}$
		- $\forall U_1, U_2 \in \mathcal{T}, U_1 \cap U_2 \subseteq \mathcal{T}$ 
		The pair $(X, \mathcal{T})$ is called a **topological space**.
	- $\mathcal{T}$ the collection of all subsets of $X$ is called the **discrete topology** on the set $X.$ and the set topological space $(X, \mathcal{T})$ is called a **discrete space**.
	- $\mathcal{T} = \{X, \emptyset\}$ is called the **indiscrete topology** and $(X, \mathcal{T})$ is said to be an **indiscrete space**.

- **Propositions**
	- if $(X, \mathcal{T})$ is a topological space : $\forall x \in X, \{x\} \in \mathcal{T} \implies \mathcal{T}$ is the discrete topology.   

## Open Sets, Closed Sets, and Clopen Sets
- **Definitions**
	- The members of $\mathcal{T}$ are said t o be **open sets**.
	- $S$ of $X$ is said to be a **closed set** in $(X, \mathcal{T})$ if its complement is $X$, namely $X \setminus S$ is open in $(X, \mathcal{T})$.
	- A subset $S$ is sad to be **colopen** if it's both open. and closed in $(X, \mathcal{T})$.

- **Propositions**
	 - in $(X, \mathcal{T})$ 
		 - the intersection of any **finite** number of open sets is an open set.
		 - the union of any **finite or infinite** number of open sets is an open set.

- **Notes**
	- In **every** topological space $(X, \mathcal{T})$ both $X$ and $\emptyset$ are **colopen**.
	- In a **discrete space** all subsets of $X$ are **colopen**.
	- In an **indiscrete space** the **only colopen** subsets are $X$ and $\emptyset$.

## The finite-closed Topology
- **Definitions**
	- $\mathcal{T}$ is called **finite-closed topology** or **cofinite topology** if the closed subsets of $X$ are $X$ and all the finite subsets of $X$.