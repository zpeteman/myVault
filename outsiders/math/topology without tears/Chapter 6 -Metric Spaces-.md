## Metric Spaces
- **Definition**
	- Let $X$ be a non-empty set and $d$ a real-valued function defined on $X\times X$ s.t for $a,b \in X$:
		- $d(a,b) \ge 0$ and $d(a,b)=0$ if and only if $a=b$
		- $d(a,b) = d(b,a)$
		- $d(a,c) \le d(a,b) + d(b,c)$
		$d$ is said to be a **metric** on $X$, $(X,d)$ is called a **metric space** and $d(a,b)$ is referred to as the **distance** between $a$ and $b$.
	- Let $(X,d)$ be a metric space and $r$ any positive real number. then the **open ball about $a \in X$ of radius $r$** is the set $B_r = \{x:x\in X,d(a,x)<r\}$
	- Metrics on a set $X$ are said to be **equivalent** if they induce the same topology on $X$.
	- A topological space is said to be a **Harsdorf space** if for each pair of distinct point $a$ and $b$ in $X$, there exist open sets $U$ and $V$ such that $a \in U, b \in V$ and $U \cap V = \emptyset$.
	- A space $(X,\mathcal{T})$ is said to be **metrizable** if there exists a metric $d$ on the set $X$ with the property that $\mathcal{T}$ is the topology induced by $d$.

- **Propositions**
	- Let $(X,d)$ be a metric space. Then the collection of open balls in $(X,d)$ is a basis for a topology $\mathcal{T}$ on $X$.
	- Let $(X,d)$ be a metric space and $\mathcal{T}$ the topology induced on $X$ by the metric $d$. Then a subset $U$ of $X$ is open in $(X,\mathcal{T})$ if and only if for each $a \in U$ there exists an $\epsilon >0$ such that the open ball $B_{\epsilon}(a) \subseteq U$. 
	- Let $(X,d)$ be any metric space and $\mathcal{T}$ the topology induced on $X$ by $d$. Then $(X,\mathcal{T})$  is Harsdorf space.

- **Lemma**
	- Let $(X,d)$ be a metric space and $a$ and $b$ points of $X$. further, let $\delta_1, \delta_2$ be positive real numbers. If $c\in B_{\delta} \subseteq B_{\delta_1}(a) \subseteq B_{\delta_2}(b)$.

- **corollaries**
	- Let $(X,d)$ be a metric space and $B_1$ and $B_2$ open balls in $(X,d)$. Then $B_1 \cap B_2$ is a union of open balls in $(X,d)$.

## Convergence of Sequences
- **Definitions**
	the sequence **converge** to $x\in \mathbb{R}$ if $\forall \epsilon > 0 \exists n_0 \in \mathbb{N} \forall n>n_0, d(x,x_n) < \epsilon$

- **Propositions**
	- if $x_n \to x$ and $x_n \to y$ then $x=y$.
	- $A$ is closed in $(X,d)$ if and only if $a_n \to x$ where $x \in X$ and $a_n \in A$ for all $n$, implies $x\in A$.

## Completeness
- **Definitions**
	- A metric space is said to be **complete** if every Cauchy sequence in the space does converges in the space.
	- A topological space $(X,\mathcal{T})$ is said to be **completely metrizable** if there exists a metric $d$ such that $\mathcal{T}$ is determined by $d$ and $(X,d)$ is a complete metric space.
	- A topological space is said to be **separable** if it has a countable dense subset.
	- A topological space is said to be **Polish space** if it separable and completely metrizable.
	- A topological space is said to be **Souslin space** if it is Hausdorff and continuous image of a Polish space. if $A$ is a subset of a topological space such that with the induced topology 2, the space $(A,\mathcal{T}_2)$ is a **Souslin space** then $A$ is said to be an **analytic set** in $(Y,\mathcal{T}_1)$.
	- let there be two metric spaces, $(X,d)$ is said to be **isometric** to $(Y,d_1)$ if there exists $f:X \to Y$  such that for all $x_1,x_2 \in X$ $d(x_1,x_2) = d_1(f(x_1),f(x_2))$. such a mapping $f$ is said to be an **isometry**.
	-  Let $(X,d)$ and $(Y,d_1)$ be metric spaces and $f$ a mapping of $X$ into $Y$. Let $Z=f(X)$ and $d_2$ be the metric of $Z$ by $d_1$. if $f: (X,d) \to (Z,d_2)$ is an isometry then $f$ is said to be an **isometric embedding** of $(X,d)$ in $(Y,d_1)$
	- $f$ is an isometric embedding between two metric spaces, if the second is complete and $f(X)$ is a dense subset of it, then it is said to be a **completion** of the first one.
	- Let $(N, || ||)$ be a normed vector space and $d$ the associated metric on the set $N$. Then $(N, ||||)$ is said to be a **Banach space** if $(N,d)$ is a complete metric space. 

- **Propositions**
	- Let $(X,d)$ be a metric space, and $(x_n)_n$ be a sequence. if there exists a point $a\in X$ such that $x_n \to a$ then the sequence is a **Cauchy sequence**.
	- Let $(X,d)$ and $(Y,d_1)$ such that $Y$ is in $X$:
		- if $(X,d)$ is complete and $Y$ is closed subspace then $(Y,d_1)$ is a complete metric space.
		- if $(Y,d_1)$ is a complete metric space, then $Y$ is a closed subspace $(X,d)$.
	- if $(X,d)$ is a metric space, then it has a completion.
	- if $X$ is a dense subset of $A$ and $Y$ a dense subset of $B$ then if there's $f$ an isometry from $X \to Y$ then there's exists an isometry $g: A \to B$ such that $g(x) = f(x), \forall x \in X$. 

- **Theorems**
	- **Bolzano-Weisrstrass Theorem**
		Every bounded sequence in $\mathbb{R}$ with the Euclidean metric has a convergent subsequence. 

- **Corollaries**
	- The metric space $\mathbb{R}$ with the euclidean metric is a complete metric space.
	- For each positive integer $m$, the metric space $\mathbb{R}^m$ with the euclidean metric is a complete metric space.

## Contraction Mappings
- **Definitions**
	- Let $f$ be a mapping of set $X$ into itself. Then a point $x \in X$ is said to be a **fixed point** of $f$ if $f(x) = x$.
	- Let $(X,d)$ be a metric space and $f$ a mapping of $X$ into itself. Then $f$ is said to be a **contraction mapping** if there exists an $r \in (0,1)$ such that $$d(f(x_1),f(x_2)) \le  r.d(x_1,x_2) \text{  } \forall x_1,x_2 \in X$$

- **Propositions**
	- Let $f$ be a contraction mapping of the metric space $(X,d)$. Then $f$ is a continuous mapping.

- **Theorems**
	- **contraction mapping theorem/ Banach fixed point theorem**
		- Let $(X,d)$ be a complete metric space and $f$ a contraction mapping of $(X,d)$ into itself. Then $f$ has precisely one fixed point.

## Baire Space
- **Definitions**
	- Let $(X,\mathcal{T})$ be any topological space and $A$ any subset of $X$. The largest open set contained in $A$ is called the **interior** of $A$ and is denoted by **int(A)**. Each point $x \in int(A)$ is called an **interior point** of $A$. the interior of the complement of $A$ is called the **exterior** of $A$ and each point in **Ext(A)** are called **exterior point** of $A$. The set $\bar{A}$ \ $int(A)$  is called **boundary** of $A$. Each point in the boundary of $A$ is called **boundary** of $A$. Each point in the boundary of $A$ is called a **boundary point** of $A$.
	- A subset $A$ of a topological space is said to be **nowhere dense** if the set $\bar{A}$ has empty interior.
	- A topological space is said to be a **Baire space** if for every sequence {$X_n$}  of open dense subsets of $X$ the set $\bigcap_1^{\infty} X_n$ is also dense in $X$. 
	- Let $Y$ be a subset of a topological space. if $Y$ is a union of a countable number of nowhere dense subsets of $X$,  then $Y$ is said to be a set of the **first category**. if $Y$ is not first category in $(X,\mathcal{T})$, it is said to be a set of the **second category** in $(X,\mathcal{T})$.
	- Let $S$ be a subset of a real vector space $V$. The set $S$ is said to be **convex** if for each $x,y \in S$ and every real number $0 <\lambda < 1$, the point $\lambda x + (1- \lambda) y$ is in $S$.

- **Propositions**
	if $Y$ is a first category subset of a Baire space $(X,\mathcal{T})$, then the  interior of $Y$ is empty.

- **Theorems**
	- **Baire Category Theorem**
		Let $(X,d)$ be a complete metric space. If $X_1,X_2, \dots,X_n, \dots$ is a sequence of open dense subsets of $X$, then the set $\bigcap_{n=1}^{\infty} X_n$ is also dense in $X$.   
	- **Open mapping Theorem**
		Let $(B, ||||)$ and $(B_1, ||||_1)$ be Banach spaces and $L:B \to B_1$ a continuous linear mapping of $B$  onto $B_1$. Then $L$ is an open mapping. 

- **Corollary**
	- Let $(X,d)$ be a complete metric space. if $X_1,X_2, \dots, X_n, \dots,$ is a sequence of subsets of $X$ s.t $X= \bigcup_1^{\infty} X_n$, then for at least one $n \in \mathbb{N}$,  the set $\bar{X_n}$ has non-empty interior; that is $X_n$ is not nowhere dense.
	- Every complete metrizable space is a Baire space.
	- if $Y$ is a first category subset of a Baire space $(X,\mathcal{T})$, then $X \setminus Y$ is a second category set.
	- A one-to-one continuous linear map of one Banach space onto another Banach space is homeomorphism. In particular, a one-to-one continuous linear map of a Banach space onto itself is a homeomorphism.