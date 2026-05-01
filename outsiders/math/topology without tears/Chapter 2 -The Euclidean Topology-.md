## The Euclidean Topology on $\mathbb{R}$
- **Definitions**
	$S$ in $\mathbb{R}$ is **Euclidean topology** on $\mathbb{R}$ : $\forall x \in S, \exists a,b \in \mathbb{R}, a<b \text{ s.t } x \in \left(a,b\right) \subseteq S$.

## Basis for a Topology
- **Definitions**
	- let $(X, \mathcal{T})$ be a topological space. A collection $\mathcal{B}$ of open subsets of $X$ is said to be a **basis** for the topology $\mathcal{T}$ if every open set is a union of members of $\mathcal{B}$. 

- **Propositions**
	- $S$ is open if and only if $S$ is the union of open intervals.
	- $\mathcal{B}$ is a basis for a topology on $X$:
		- $X = \bigcup_{B \in \mathcal{B}} B$
		- $\forall B_1,B_2 \in \mathcal{B}, B_1 \cap B_2$ is a union of members of $\mathcal{B}$.

## Basis for a Given Topology
- **Propositions**
	- let $(X, \mathcal{T})$, let $\mathcal{B}$ be a family of open subsets of $X$ is a basis for $\mathcal{T}$ if and only if for any point $x$ belonging to any open set $U$, there is a $B \in \mathcal{B}$ s.t  $x\in B \subseteq U$.
	- $U$ of $X$ is open if and only if for each $x\in U$ there exists a $B \in \mathcal{B}$ such that $x\in B \subseteq U$.
	- Let $\mathcal{B}_1, \mathcal{B}_2$ be bases for $\mathcal{T}_1, \mathcal{T}_2$. $\mathcal{T}_1 =  \mathcal{T}_2$ if and only if :
		- $\forall x \in B \in \mathcal{B}_1, x \in B' \subseteq B$ s.t $B' \in \mathcal{B}_2$.
		- $\forall x \in B \in \mathcal{B}_2, x \in B' \subseteq B$ s.t $B' \in \mathcal{B}_1$.
