## Compact Spaces
- **Definitions**
	- Let $A$ be a subset of a topological space $(X,\mathcal{T})$. Then $A$ is said to be **compact** if for every set $I$ and every family of open sets, $O_i, i \in I$, s.t $A \subseteq \bigcup_{i\in I} O_i$ there exists a finite subfamily $O_{i_1} , O_{i_2}, \dots, O_{i_n}$ s.t $A \subseteq O_{i_1} \cup O_{i_2} \cup \dots \cup O_{i_n}$.  
	- Let $I$ be a set and $0_i, i \in I$ a family of subset of $X$. Let $A$ be a subset of $X$. Then $0_i,i\in I$, is said to be a **covering** of $A$ if $A\subseteq \bigcup_{i \in I} O_i$. if each $O_i,i \in I$ is an open set in $(X,\mathcal{T})$, then $O_i,i\in I$ is said to be an **open covering** of $A$ if $A \subseteq \bigcup_{i\in I} O_i$. A finite subfamily is also called **finite subcovering** if $A\subseteq O_{i_1} \cup O_{i_2} \cup \dots \cup O_{i_n}$.
	- A subset $A$ of a topological space $(X,\mathcal{T})$ is said to be **compact** if every open covering of $A$ has a finite subcovering. If the compact subset $A$ equals $X$, then $(X,\mathcal{T})$ is said to be a **compact space**.

- **Propositions**
	The closed interval $[0,1]$ is compact. 

## The Heine-Borel Theorem
- **Definitions**
	- A subset $A$ of a metric space $(X,d)$ is said to be **bounded** if there exists a real number $r$ such that $d(a_1,a_2) \le r$, for  all $a_1$ and $a_2$ in $A$.
- **Propositions**
	- Let $f:(X,\mathcal{T}) \to (Y,\mathcal{T}_1)$ be continuous surjective map. if $(X,\mathcal{T})$ is compact, then $(Y,\mathcal{T}_1)$ is compact.
	- Every closed subset of a compact space is compact.
	- A compact subset of a Hausdorff topological space is closed.
	- A compact subset of $\mathbb{R}$ is bounded.
	- Every compact subset of $\mathbb{R}$ is closed and bounded.
	- Let $A$ be a compact subset of a metric space $(X,d)$. Then $A$ is closed and bounded.
	- Let $(X,\mathcal{T})$ be a compact space and $f$ a continuous mapping from $(X,\mathcal{T})$ into $\mathbb{R}$. Then the set $f(X)$ has a greatest element and a least element.
	- Let $a$ and $b$ be in $\mathbb{R}$ and $f$ a continuous function from $[a,b]$ into $\mathbb{R}$. Then $f([a,b]) = [c,d]$, for some $c$ and $d$ in $\mathbb{R}$. 

- **Theorem**
	- **Heine-Borel Theorem**
		Every closed bounded subset of $\mathbb{R}$ is compact.
	- **generalised Heine-Borel Theorem**
		A subset of $R^n,n \ge 1$ is compact if and only if it is closed and bounded. 

- **corollaries**
	- Let $(X,\mathcal{T})$ and $(Y,\mathcal{T}_1)$ be homoeomorphic topological spaces. if $(X,\mathcal{T})$ is compact, then $(Y,\mathcal{T}_1)$ is compact.
	- for $a$ and $b$ in $\mathbb{R}$ with $a<b$, $[a,b]$ is compact while $(a,b)$ is not compact.
	- A compact subset of a metrizable space is closed.