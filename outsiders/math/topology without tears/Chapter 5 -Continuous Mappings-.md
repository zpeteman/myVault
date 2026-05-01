## Continuous Mappings
- **Definitions**
	Let $(X,\mathcal{T}) , (Y, \mathcal{T}')$ and $f: X \to Y$. Then $f: (X,\mathcal{T}) \to (Y, \mathcal{T}')$ is said to be a **continuous mapping** if $\forall U \in \mathcal{T}', f^{-1}(U) \in \mathcal(T)$.

- **Propositions**
	- Let $f: (X,\mathcal{T}) \to (Y, \mathcal{T}')$. Then $f$ is continuous if and only if $\forall x \in X, \forall U \in \mathcal{T}'$ with $f(x) \in U, \exists V \in \mathcal{T} \text{ s.t } x\in V , f(V) \subseteq U$.  
	- Let $(X,\mathcal{T}), (Y, \mathcal{T}_1), (Z, \mathcal{T}_2)$ if $f: (X,\mathcal{T}) \to (Y, \mathcal{T}_1)\text{ and } g: (X,\mathcal{T}_1) \to (Z, \mathcal{T}_2)$ are continuous mappings, then the composite function $g \circ f: (X,\mathcal{T}) \to (Z, \mathcal{T}_2)$ is continuous.
	- $f$ is continuous if and only if for every closed subset $S$ of $Y$, $f^{-1}(S)$ is a closed subset of $X$.
	- $f$ is homeomorphism if and only if :
		- $f$ is continuous
		- $f$ is bijective hens inversed
		- the inverse is continuous

- **Lemma**
	 - Let $f: \mathbb{R} \to \mathbb{R}$ then $f$ is continuous if and only if $\forall a \in \mathbb{R} \forall U$ containing $f(a)$, $\exists V$ an open set containing $a$ s.t $f(V) \subseteq U$.
	  - Let $f: (X,\mathcal{T}) \to (Y, \mathcal{T}')$
		  - $\forall U \in \mathcal{T}', f^{-1}(U) \in \mathcal{T}$
		  - $\forall a \in X ,\forall U \in \mathcal{T}', f(a) \in U \exists V \in \mathcal{T} \text{ s.t } a \in V f(V) \subseteq U$.

## Intermediate Value Theorem
- **Definitions**
	A topological space is said to be **path-connected** if for each pair of points $a$ and $b$ of $X$ there exists a continuous mapping $f: [0,1] \to (X,\mathcal{T})$, such that $f(0) = a$ and $f(1) = b$. The mapping $f$ is said to be a **path joining $a$ to $b$**.

- **Propositions**
	- if $f$ is **surjective and continuous** then if $(X,\mathcal{T})$ is connected, then $(Y,\mathcal{T}_1)$ is connected.
	- Every path-connected space is connected.

- **Theorems**
	Let $f: [a,b] \to \mathbb{R}$ be continuous and let $f(a) \ne f(b)$. Then for every number $p$ between $f(a)$ and $f(b)$ there is a point $c \in [a,b]$ s.t $f(c) = p$.

- **corollaries**
	- if $f:[a,b] \to \mathbb{R}$ is continuous and s.t $f(a) >0$ and $f(b)<0$, then there exists an $x\in [a,b]$ s.t $f(x)=0$.
	- Let $f$ be a continuous mapping of $[0,1] \to [0,1]$. then there exists a $z\in[0,1]$ s.t $f(z)=z$ ($z$ is a called **fixed point**)