---
aliases:
  - chapter_I
---

## 📚 Course Structure
- Section 1: **Vector Spaces**
- Section 2: **Linear Maps**

---
## 📐 Equations & Concepts
#### Vector Spaces:
- **Definition:**
	A vector space over a field $K$ ($\mathbb{R}$ or $\mathbb{C}$) is a set $E$ with:
	- **Addition:** $E$ is a commutative group under addition.
	- **Scalar multiplication:** For $\lambda \in K, x \in E$, $\lambda x \in E$, satisfying:
		1. $1x = x$
		2. $\lambda(x + y) = \lambda x + \lambda y$
		3. $(\lambda + \mu)x = \lambda x + \mu x$
		4. $(\lambda\mu)x = \lambda(\mu x)$
- **Examples:**
	- $\mathbb{R}^n$ is a vector space over $\mathbb{R}$.
	- $\mathbb{C}$ is a vector space over $\mathbb{R}$, but $\mathbb{R}$ is not over $\mathbb{C}$.
	- The set of polynomials $K[X]$ is a vector space over $K$.
	- The set of functions from a set $I$ to $\mathbb{R}$ is a vector space over $\mathbb{R}$.

- **Subspaces:**
	A subset $F \subset E$ is a subspace if it's a vector space under the same operations.
	- $\{0\}$ and $E$ are always subspaces.
	- The intersection of subspaces is a subspace; the union is not always.

- **Linear Combination:**
	A vector $v$ is a linear combination of $v_1, ..., v_n$ if $v = \lambda_1 v_1 + ... + \lambda_n v_n$ for scalars $\lambda_i$.

- **Span:**
	The set of all linear combinations of $v_1, ..., v_n$ is called their span, denoted $\text{Vect}(v_1, ..., v_n)$.

- **Generating Set:**
	A set $v_1, ..., v_n$ generates $E$ if $\text{Vect}(v_1, ..., v_n) = E$.

- **Linear Independence:**
	$v_1, ..., v_n$ are linearly independent if $\lambda_1 v_1 + ... + \lambda_n v_n = 0$ implies all $\lambda_i = 0$.
	Otherwise, they are dependent.
	- A set is dependent iff one vector is a linear combination of the others.

- **Basis & Dimension:**
	A basis is a set that is both linearly independent and generating. All bases have the same number of elements, called the dimension.
	- In $K^n$, the standard basis is $e_1 = (1,0,...,0), ..., e_n = (0,...,1)$.
	- $\dim_K K^n = n$.
	- A vector space is finite-dimensional if it has a finite basis.

- **Rank:**
	The rank of a set of vectors is the dimension of their span.

- **Sum of Subspaces:**
	For subspaces $F, G$, their sum is $F + G = \{x + y \mid x \in F, y \in G\}$.
	- The sum is direct ($F \oplus G$) if every element has a unique decomposition.
	- $F \cap G = \{0\}$ iff the sum is direct.
	- $\dim(F + G) = \dim F + \dim G - \dim(F \cap G)$.

#### Linear Maps:
- **Definition:**
	A function $f: E \to E'$ is linear if:
	- $f(v + w) = f(v) + f(w)$
	- $f(\lambda v) = \lambda f(v)$
	If $f$ is bijective, it's an isomorphism.

- **Image & Kernel:**
	- $\text{Im} f = \{f(v) \mid v \in E\}$ is a subspace of $E'$.
	- $\ker f = \{v \in E \mid f(v) = 0\}$ is a subspace of $E$.
	- $f$ is injective iff $\ker f = \{0\}$.

- **Dimension Theorem:**
	If $E$ is finite-dimensional and $f: E \to E'$ is linear:
	$$
	\dim E = \dim \ker f + \dim \text{Im} f
	$$

---
## 📝 Notes
- Vector spaces generalize the idea of vectors to any field.
- Subspaces must contain 0, be closed under addition and scalar multiplication.
- A basis allows unique representation of every vector.
- The rank tells you the maximum number of linearly independent vectors in a set.
- Linear maps preserve vector space structure; their kernel and image are always subspaces.
- The dimension theorem links the size of the kernel and image to the whole space.