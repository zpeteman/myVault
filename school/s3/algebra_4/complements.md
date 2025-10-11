---
aliases:
  - Chapter_0
---

## 📚 Course Structure
- Section 1: **Groups**
- Section 2:  **Rings, Homomorphisms and Ideals**
---
## 📐 Equations & Concepts
#### Groups:
- **Groups**:
	let $E$ be a non empty set and let $*$ be an operation in $E$. $(E,*)$ is a group if :
	- $*$ is associative.
	- $*$ if a neutral element.
	- $\forall x \in E, \exists x' \in E ; x* x' = x'*x=e$. 
	if $*$ is commutative then the group $(E,*)$ is a commutative group.
- **symmetrical groups:**
	let $n \in \mathbb{N}^*$ and $\mathbb{N}_n = \{1,2,3, \dots, n\}$, we call permutation of $\mathbb{N}_n$, all bijective functions $f: \mathbb{N}_n \to \mathbb{N}_n$ and noted and noted $S_n$. the set of all permutations of $\mathbb{N}_n$  
	- $Card(S_n) = n!$ 
	- $\sigma \in S_n$ is : $$
	\begin{bmatrix}
1 & 2 & \dots & n \\
\sigma(1) & \sigma(2) & \dots & \sigma(n)
\end{bmatrix}$$
	- we use $\sigma_1  \sigma_2$ instead of $\sigma_1 o \sigma_2$.
	- $S_1,S_2$ are commutative but this proposition is not true for $S_{n,n>2}$. ($\sigma, \phi \in S_{n,n>2}, \sigma \phi \neq \phi \sigma$)
	- **permutation:**
		let $\sigma \in S_n, n \ge 2$, we say that $\sigma$ is **permutation** if there's $i,j \in \mathbb{N}_n, i \neq j$ 
		- $\sigma(i) = j$ and $\sigma(j) = i$.
		- $\sigma(k) = k, \forall k \in \mathbb{N}_n\ \{i,j\}$ and we note $\sigma_{i,j}$.
	- :
		let $(i,j) \in \mathbb{N}_n^2$ we say that the couple $(i,j)$ is an inversion of $\sigma$, 
		if $i<j, \sigma(i)>\sigma(j)$.
		- the number of **inversions** of $\sigma$ is noted $I(\sigma)$, signature of $\sigma$ is noted $\epsilon(\sigma)$ the number $\epsilon(\sigma)=(-1)^{I(\sigma)}$. 
		
#### Rings, Homomorphisms and Ideals:
- **Rings:***
	A **ring** is a set $A$ equipped with two binary operations:
	- addition
	- multiplication
	such that:
	-  $(A,+)$ is an abelian group,
	-  multiplication is associative,
	-  $a(b+c) = ab + ac, \quad (b+c)a = ba + ca, \quad \forall a,b,c \in A.$
	
	If multiplication is commutative, the ring $(A,+,\cdot)$ is called a **commutative ring**.  
	If $A$ has a multiplicative identity $1$ (a neutral element for multiplication), then $(A,+,\cdot)$ is called **unitary ring**.
- **Subring:**
	Let $A$ be a ring. A subset $B \subset A$ is called a **subring** of $A$ if:
	-  $B$ is a subgroup of $(A,+)$,
	-  $B$ is closed under multiplication: $\forall x,y \in B, \; xy \in B$.
	Equivalently, $B$ is a subring of $A$ :
    -  $B \neq \varnothing$,
    -  $\forall x,y \in B, \; x-y \in B$,
     - $\forall x,y \in B, \; xy \in B$.
- **Homomorphisms and Ideals:**
	- Let $A$ and $A'$ be two rings. A map $f: A \to A'$ is called a **ring homomorphism** if for all $x, y \in A$:
		- $f(x + y) = f(x) + f(y)$
	    - $f(x \cdot y) = f(x) \cdot f(y)$
	- A subset $I$ of a commutative ring $A$ is called an **ideal** of $A$ if:
	    -  $(I, +)$ is a subgroup of $(A, +)$
	     - $\forall a \in A, \; \forall x \in I, \; ax \in I$
    - An integral domain (or **integral ring**) $A$ is a commutative ring such that for all $x, y \in A$: $xy = 0_A \implies x = 0_A \text{ or } y = 0_A$.
    -  Let $A$ be a commutative ring. An ideal $I$ of $A$ is called **principal** if there exists an element $x \in I$ such that $I = \{ ax \mid a \in A \}$.
    We write $I = (x)$ or $I = Ax$.
    - A commutative integral ring $A$ is called a **principal ideal ring** if all its ideals are principal.
---

## 📝 Notes
- $(S_n,o)$ is called a **symmetrical group/ permutation group of** $\mathbb{N}_n$.
- $\sigma_{i,j} \sigma_{i,j} =id\mathbb{N}_n$. 
- Let $t_i$ be the number of inversions relative to $i$, that is, $t_i$ is the number of $j \in \{i+1, \dots, n\}$ such that $\sigma(j) < \sigma(i)$. It is clear that $I(\sigma) = \sum_{i=1}^{n-1} t_i.$
- Let $\sigma \in S_n$, we have $\epsilon (\sigma) = \Pi_{1\le i < j\le n} \frac{\sigma(j) - \sigma(i)}{j- i}$.
 