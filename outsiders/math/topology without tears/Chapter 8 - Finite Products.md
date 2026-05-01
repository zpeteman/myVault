## The Product Topology
- **Definitions**
	Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2), \dots, (X_n,\mathcal{T}_n)$ be topological spaces. Then the **product topology** $\mathcal{T}$ on the set $X_1 \times X_2 \times \dots \times X_n$ is the topology having the family {$O_1 \times O_2 \times \dots \times O_n, O_i \in \mathcal{T_i}, i = 1, \dots,n$}.   

- **Propositions**
	- Let $\mathcal{B_1},\mathcal{B_2}, \dots, \mathcal{B_n}$ be bases for the topological spaces $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2), \dots, (X_n,\mathcal{T}_n)$, respectively. Then the family of sets {$O_1 \times O_2 \times \dots \times O_n:  O_i \in \mathcal{B}_i, i=1, \dots , n$} is a basis for the product topology on $X_1 \times X_2 \times \dots \times X_n$.
	- Let $C_1,C_2,\dots, C_n$ be closed subsets of the topological spaces $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2), \dots ,(X_n,\mathcal{T}_n)$, respectively. Then $C_1 \times C_2 \times \dots \times C_n$ is a closed subset of the product space $(X_1\times X_2 \times \dots \times X_n,\mathcal{T})$.

## Projections Onto Factors of a Product
- **Definitions**
	- let $\mathcal{T_1}$ and $\mathcal{T_2}$ be topologies on a set $X$. Then $\mathcal{T_1}$ is said to be a **finer topology** than $\mathcal{T_2}$ (and $\mathcal{T_2}$ is said to be a **coarser topology** than $\mathcal{T_1}$) if $\mathcal{T_2} \subseteq \mathcal{T_1}$.
	- Let $(X,\mathcal{T})$ and $(Y,\mathcal{T}_1)$ be topological spaces and $f$ a mapping from $X$ into $Y$. Then $f$ is said to be an **open mapping** if for every $A \in \mathcal{T}, f(A) \in \mathcal{T_1}$. The mapping $f$ is said to be a **closed mapping** if for every closed set $B$  in $(X,\mathcal{T})$, $f(B)$ is closed in $(Y,\mathcal{T}_1)$.

- **Propositions**
	- Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n)$ be topological spaces and $(X_1 \times X_2 \times \dots \times X_n,\mathcal{T})$ their product space.
		for each $i \in \{1,\dots, n\}$ let $p_i: X_1 \times X_2 \times \dots \times X_n \to X_i$ be the projection mapping; that is, $p_i(<x_1,x_2,\dots,x_i,\dots,x_n>) =x_i$ for each $<x_1,x_2,\dots, x> \in X_1 \times X_2 \times \dots \times X_n$. Then
		- each $p_i$ is a continuous surjective open mapping
		- $\mathcal{T}$ is the coarsest topology on the set $X_1 \times X_2 \times \dots \times X_n$ such that each $p_i$ is continuous.
	- Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}),\dots , (X_n,\mathcal{T}_n)$ be topological spaces and ($X_1 \times X_2 \times \dots \times X_n, \mathcal{T}$) the product space. Then each $(X_i,\mathcal{T}_i)$ is homoeomorphic to a subspace of $(X_1 \times X_2 \times \dots \times X_n,\mathcal{T})$.

- **corollary**
	for $n \ge 2$ the projection mappings of $\mathbb{R}^n$ onto $\mathbb{R}$ are continuous open mapping.

## Tychonoff's Theorem for Finite Products
- **Propositions**
	Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n)$ be topological spaces. If $\Pi_1^n(X_i,\mathcal{T}_i)$ is compact then each $(X_i,\mathcal{T}_i)$ is compact.

- **Theorems**
	- **Tychonoff's Theorem for Finite Products**
		if $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n)$ are compact spaces, then $\Pi_1^n(X_i,\mathcal{T}_i)$ is a compact space.
	- **Generalised Heine-Borel Theorem**
		A subset of $\mathbb{R^n},n\ge1$ is compact if and only if it is closed and bounded.

## Products and Connectedness
- **Definitions**
	- Let $(X,\mathcal{T})$ and let $x$ be any point in $X$. The **component in $X$ of $x$, $C_X(x)$**, is defined to be the union of all connected subsets of $X$ which contain $x$.
	- A topological space is said to be a **continuum** if it is compact and connected.

- **Propositions**
	- Let $x$ be any point in a topological space $(X,\mathcal{T})$. Then $C_X(x)$ is connected.
	- Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n)$ be topological spaces. then $\Pi_1^n(X_i,\mathcal{T}_i)$ is connected if and only if each $(X_i,\mathcal{T}_i)$ is connected.
	- Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n)$ be topological spaces. Then $\Pi_1^n(X_i,\mathcal{T}_i)$ is a continuum if and only if each $(X_i,\mathcal{T}_i)$ is a continuum.

- **Lemmas**
	Let $a$ and $b$ be points in $(X,\mathcal{T})$. If there exists a connected set $C$ containing both $a$ and $b$ then $C_X(a)=C_X(b)$.

## Fundamental Theorem of Algebra
- **Theorems**
	- **The fundamental Theorem of Algebra**
		Every Polynomial $f(z)=a_nz^n + a_{n-1}z^{n-1}+\dots+a_1z +a_0$ where each $a_i$ is a complex number, $a_n \neq 0$, and $n\ge 1$, has a root; that is, there exists a complex $z_0$ s.t $f(z_0) = 0$.