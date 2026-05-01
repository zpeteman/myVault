## The Cantor Set

## The Product Topology
- **Definitions**
	Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n),\dots$ be a countably infinite family of topological spaces. Then the product $\Pi_1^{\infty}X_i$, of the sets $X_i,i\in \mathbb{N}$ consists of all infinite sequences $<x_1,x_2,\dots,x_n,\dots>$, where $x_i \in \mathbb{N}$ for all $i$ the **product space**, $\Pi_1^{\infty}(X_i,\mathcal{T}_i)$, consists of the product $\Pi_1^{\infty}X_i$ with the topology $\mathcal{T}$ having as its basis the family $$B=\{\Pi_1^{\infty}O_i: O_i \in \mathcal{T_i} \text{ and } O_i=X_i \text{ for all but a finite number of } i\}$$ The topology $\mathcal{T}$ is called the **product topology**.

- **Propositions**
	- Let $(X_1,\mathcal{T}_1),(X_2,\mathcal{T}_2),\dots,(X_n,\mathcal{T}_n),\dots$ 
		be a countably infinite family of topological spaces and their product space. For each $i$, let $p_i: \Pi_1^{\infty} X_j \to X_i$ be the projection mapping; that is $p_i(<x_1,x_2,\dots,x_n,\dots>)=x_i$ for each $<x_1,x_2,\dots,x_n,\dots>\in \Pi_1^{\infty}X_j$. 
		- each $p_i$ is continuous surjective open mapping
		- $\mathcal{T}$ is the coarsest topology on the set $\Pi_1^{\infty}X_j$ s.t each $p_i$ is continuous.
	- Let $(X_i,\mathcal{T}_i)$ and $(Y_i,\mathcal{T'}_i), i \in \mathbb{N}$ be countably infinite families of topological spaces having product spaces and, respectively. if the mapping $h_i:(X_i,\mathcal{T}_i) \to (Y_i,\mathcal{T'}_i)$ is continuous for each $i \in \mathbb{N}$, then so is the mapping $h:\Pi_1^{\infty}X_i,\mathcal{T} \to \Pi_1^{\infty}Y_i,\mathcal{T'}$ given by $h:\Pi_1^{\infty} = \Pi_1^{\infty}h_i(x_i)$; that is, $h(<x_1,x_2,\dots,x_n,\dots>)=<h_1(x_1),h_2(x_2),\dots,h_n(x_n),\dots>$. 

## The Cantor Space and The Hilbert Cube
- **Definitions**
	Fore each positive integer $n$, let the topological space $(I_n,\mathcal{T}_n)$ be homoeomorphic to $[0,1]$. Then the product space $\Pi_1^{\infty}(I_n,\mathcal{T}_n)$ is called the **Hilbert cube** and is denoted by $I^{\infty}$. The product space $\Pi_1^n(I_i,\mathcal{T}_i)$ is called the **n-cube** and is denoted by $I^n$,for each $n\in \mathbb{N}$.

- **Propositions**
	- Let $(G_i,\mathcal{T}_i),i\in \mathbb{N}$, be a countably infinite family of topological spaces each of which is homoeomorphic to the Cantor Space $(G,\mathcal{T})$. Then $$(G,\mathcal{T}) \cong \Pi_1^{\infty}(G_i,\mathcal{T}_i) \cong \Pi_1^{n}(G_i,\mathcal{T}_i) \text{ for each } n \in \mathbb{N}$$
	- The topological space $[0,1]$ is a continuous image of the Cantor Space $(G,\mathcal{T})$.
	- Let $(X_i,\mathcal{T}_i), i\in \mathcal{N}$ be a countably infinite family of metrizable spaces. Then $\Pi_1^{\infty}(X_i,\mathcal{T}_i)$ is metrizable.
	- Let $(X_i,\mathcal{T}_i), i\in \mathbb{N}$, be a countably infinite family of completely metrizable spaces. Then $\Pi_1^{\infty}(X_i,\mathcal{T}_i)$ is completely metrizable.

- **Theorem**
	- The Hilbert cube is compact.

- **Corollaries**
	- The Hilbert cube is metrizable.

## Urysohn's Theorem
- **Definitions**
	- 