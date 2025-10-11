---
aliases:
  - Chapter_I
---
## 📚 Course Structure
- Section 1: **Eigenvectors and Eigenvalues**
- Section 2:  **Characteristic Polynomials**
- Section 3: **Reduction to Triangular Form**
- Section 4: **Diagonalization**
---
## 📐 Equations & Concepts
#### Eigenvectors and Eigenvalues:
- **Definition:**
	Let  be a vector space over $K$ and $u \in \text{End}(E)$.
	- A vector $ x \in E$ is called an **eigenvector** of $u$ if $x \neq 0$ and there exists $\lambda \in K$ such that $u(x) = \lambda x$. Such a $\lambda$ is unique because $\lambda x = \lambda' x$ implies  $(\lambda - \lambda')x = 0$, so $\lambda = \lambda'$ since $x \neq 0$.
	- A scalar $\lambda$ is called an **eigenvalue** of $u$ if there exists a vector $x \neq 0$ such that $u(x) = \lambda x$. (In this case, $x$ is an eigenvector of $u$.) Equivalently, $x \in \text{Ker}(u - \lambda \text{Id}_E) \setminus \{0\}$.
	- The subspace $F_\lambda$ of $E$ defined by $F_\lambda = \text{Ker}(u - \lambda \text{Id}_E)$ is called the **eigenspace** of $E$ associated with $\lambda$.
	Therefore, $\lambda$ is an eigenvalue of $u$ if and only if $F_\lambda \neq \{0\}$.
- **Criterion:**
	Let $u \in \text{End}(E)$, where $E$ is a finite-dimensional vector space over $K$. A scalar $\lambda \in K$ is an eigenvalue of $u$ **if and only if** $\det(u - \lambda \text{Id}_E) = 0$.
- **corollary:**
	Let $x_1, \dots, x_p$ be eigenvectors associated with distinct eigenvalues of $u \in \text{End}(E)$.  
	Then $x_1, \dots, x_p$ are **linearly independent**.
#### Characteristic Polynomials:
- **Definition:**
	Let $E$ be a vector space of dimension $n \geq 1$ over $K$, and $u \in \text{End}(E)$. If $(e_1, \dots, e_n)$ is a basis of $E$, consider the matrix $H = (a_{ij})$ of $u$ with respect to this basis.
	For all $\lambda \in K$, the endomorphism $u - \lambda \text{Id}_E$ has matrix $H - \lambda I_n$ in the basis $(e_1, \dots, e_n)$: $$
H - \lambda I_n = 
\begin{pmatrix}
a_{11} - \lambda & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} - \lambda & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & \cdots & a_{nn} - \lambda
\end{pmatrix}
= (a_{ij} - \lambda \delta_{ij})_{i,j},
$$where $$\delta_{ij} = 
\begin{cases}
1 & \text{if } i = j, \\
0 & \text{if } i \neq j.
\end{cases}
$$
	The eigenvalues of $u$ are obtained using the criterion from §1 by writing the relation $\det(u - \lambda \text{Id}_E) = 0$, which is equivalent to:$$\det(H - \lambda I_n) = 0 \quad (1)$$
	Let $X$ be an indeterminate over $K$. Consider the matrix:$$
H - X I_n = 
\begin{pmatrix}
a_{11} - X & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} - X & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & \cdots & a_{nn} - X
\end{pmatrix}
= (a_{ij} - \delta_{ij} X)_{i,j}$$
	The determinant of this matrix is:$$
P_H(X) = \sum_{\sigma \in S_n} \varepsilon(\sigma)(a_{1\sigma(1)} - \delta_{1\sigma(1)}X) \cdots (a_{n\sigma(n)} - \delta_{n\sigma(n)}X), \quad (2)$$
	where $S_n$ is the symmetric group of permutations of $\{1, \dots, n\}$, and $\varepsilon(\sigma)$ is the signature of $\sigma$.
	$P_H(X) \in K[X]$ is called the **characteristic polynomial** of the matrix $H$. Relation (1) shows that the eigenvalues of $H$ are the roots of the equation: $$P_H(\lambda) = 0. \quad (3)$$
- **Form of the Characteristic Polynomial:**
	- **proposition:**
		We have: $$
\det(H - X I_n) = (-1)^n X^n + (-1)^{n-1}(a_{11} + \cdots + a_{nn}) X^{n-1} + \cdots + \det H. \quad (1)$$
	- **Definition:**
		Let \( H = (a_{ij}) \) be an \( n \times n \) matrix. The scalar $$ 
\operatorname{tr}(H) = a_{11} + a_{22} + \cdots + a_{nn}$$ 
		is called the **trace** of the matrix $H$.This is, up to sign, the coefficient of $X^{n-1}$ in the characteristic polynomial of $H$. → In particular, two similar matrices have the same trace. This allows us to define the **trace of an endomorphism** $u$ as the trace of its matrix $H_u$ in any basis: $$\operatorname{tr}(u) = \operatorname{tr}(H_u)$$

#### Reduction to Triangular Form:
- **Definition:**
	- An endomorphism $u$ is said to be **triangularizable** if there exists a basis $B = (e_1, \dots, e_n)$ of $E$ such that the matrix of $u$ in $B$ is **upper triangular**, i.e.,$$ M(u, B, B) =
  \begin{pmatrix}
  \lambda_{11} & \lambda_{12} & \cdots & \lambda_{1n} \\
  0 & \lambda_{22} & \cdots & \lambda_{2n} \\
  \vdots & \vdots & \ddots & \vdots \\
  0 & 0 & \cdots & \lambda_{nn}
  \end{pmatrix}$$, which corresponds to: $$ 
 \begin{aligned}
  u(e_1) &= \lambda_{11} e_1, \\
  u(e_2) &= \lambda_{12} e_1 + \lambda_{22} e_2, \\
  &\vdots \\
  u(e_n) &= \lambda_{1n} e_1 + \lambda_{2n} e_2 + \cdots + \lambda_{nn} e_n.
  \end{aligned}
	  $$This means that $u(e_i) \in \text{span}(e_1, \dots, e_i)$.
	- A square matrix is said to be triangularizable if it is similar to an upper triangular matrix.
	- $u$ is said to be **diagonalizable** if there exists a basis $B$ of $E$ such that the matrix of $u$ in the basis $B$ is diagonal, i.e., $$
  M(u, B, B) = 
  \begin{pmatrix}
  \lambda_1 & 0 & \cdots & 0 \\
  0 & \lambda_2 & \cdots & 0 \\
  \vdots & \vdots & \ddots & \vdots \\
  0 & 0 & \cdots & \lambda_n
  \end{pmatrix},$$where $u(e_i) = \lambda_i e_i$ and $\lambda_i \in K$ for $1 \leq i \leq n$.
  - **Theorem:**
	Let $E$ be a finite-dimensional $K$-vector space and $u \in \text{End}(E)$. Then $u$ is triangularizable **if and only if** $u$ has all its eigenvalues in $K$.

#### Diagonalization
Let $E$ be a finite-dimensional $K$-vector space with $\dim E = n > 0$, and $u \in \text{End}(E)$.
Let $\lambda_1, \dots, \lambda_p$ be the distinct eigenvalues of $u$ in $K$, and $n_1, \dots, n_p$ their orders of multiplicity (as roots of the characteristic polynomial).
With the previous notations, $u$ is diagonalizable **if and only if** the following two conditions are satisfied:
-  $n_1 + n_2 + \cdots + n_p = n$  
-  $\dim F_{\lambda_i} = n_i$ for $1 \leq i \leq p$.

---
## 📝 Notes
- Let $\lambda$ be an eigenvalue of $u$. If $x \in F_\lambda$, then $u(x) \in F_\lambda$.
- Let $\lambda_1, \dots, \lambda_p$ be pairwise distinct eigenvalues of $u$, and let $F = F_{\lambda_1} + \dots + F_{\lambda_p}$ Then $F$ is the **direct sum** of the $F_{\lambda_i}$.
- **Two similar matrices** have **the same characteristic polynomial**.
- If $K$ is algebraically closed, condition $(a)$ is automatically satisfied.
