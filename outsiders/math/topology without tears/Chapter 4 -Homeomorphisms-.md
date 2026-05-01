## Subspaces
- **Definitions**
	- Let $Y$ be a subset of a topological space, the collection $\mathcal{T}_Y = \{O\cap Y : O \in \mathcal{T}\}$ is a topology on $Y$ called the **subspace topology**. The topological space ($Y, \mathcal{T}_Y$) is said to be a **subspace** of ($X, \mathcal{T}$).

## Homeomorphisms
- **Definitions**
	- ($Y, \mathcal{T}_1$) and ($X, \mathcal{T}$) are said to be **homoeomorphic** if there's a function $f : X \to Y$ s.t:
		- $f$ is bijective
		- $\forall U \in \mathcal{T}_1, f^{-1}(U) \in \mathcal{T}$ 
		- $\forall V \in \mathcal{T}, f(V) \in \mathcal{T}_1$
		$f$ is said to be **homoeomorphic** and we are ($Y, \mathcal{T}_1$) $\cong$ ($X, \mathcal{T}$).

## Non-Homoeomorphic Spaces
- **Definitions**
	- A subset of $S$ of $\mathbb{R}$ is said to be an **interval** if : $x\in S, z \in S, y\in \mathbb{R} \text{ s.t } s<y<z \implies y\in S$

- **Propositions**
	- Any topological space homoeomorphic to a connected space connected
	- A subspace $S$ of $\mathbb{R}$ is connected if and only if it is an interval.

- **Corollaries**
	- if $a,b,c,d \in \mathbb{R}$:
		- $(a,b) \ne [c,d)$ 
		- $(a,b) \ne [c,d]$
		- $[a,b) \ne [c,d]$
