---
aliases:
  - chapter_II
---
## 📚 Course Structure

- Section 1: **Endomorphism Algebra**
- Section 2: **Minimal Polynomial**
- Section 3: **Characteristic Polynomial**
- Section 4: **Decomposition Theorems**
- Section 5: **Diagonalization and Trigonalization**

---

## 📐 Equations & Concepts

#### Section 1: Endomorphism Algebra

- **Definition of Endomorphism:** Let $E$ be a $K$-vector space of finite dimension. An endomorphism $u$ of $E$ is a linear map from $E$ to itself: $u \in \text{End}(E)$.
    
- **Composition Properties:** For all $u, v \in \text{End}(E)$ and $(m, n) \in \mathbb{N}^2$: $$u^m \circ u^n = u^{m+n}$$
    
- **Polynomial Evaluation:** Let $P = \sum_{i=0}^{n} a_i X^i \in K[X]$ be a polynomial. We can evaluate it at an endomorphism: $$P(u) = \sum_{i=0}^{n} a_i u^i \in \text{End}(E)$$
    
- **Evaluation Map:** The map $\Phi: K[X] \to \text{End}(E)$ defined by $\Phi(P) = P(u)$ is a ring homomorphism.
    

#### Section 2: Minimal Polynomial

- **Kernel of Evaluation:** $$\ker(\Phi) = {P \in K[X] \mid P(u) = 0}$$ This is a principal ideal in $K[X]$.
    
- **Definition of Minimal Polynomial:** The minimal polynomial $\Pi_u$ of $u$ is the unique monic polynomial that generates $\ker(\Phi)$:
    
    - $\Pi_u(u) = 0$
    - $\Pi_u$ is monic (leading coefficient = 1)
    - For any $P \in K[X]$: $P(u) = 0 \Leftrightarrow \Pi_u \mid P$
    - $\Pi_u$ is the monic polynomial of smallest degree such that $\Pi_u(u) = 0$
- **Key Properties:**
    
    - If $P(u) = 0$, then $\Pi_u \mid P$
    - $\deg(\Pi_u) \leq n$ where $n = \dim(E)$
    - If $P, Q \in K[X]$ with $Q(u) = 0$, then $\ker(P(u)) \subseteq \ker(Q(u))$

#### Section 3: Characteristic Polynomial

- **Characteristic Polynomial Definition:** Let $A$ be the matrix of $u$ in some basis. The characteristic polynomial is: $$\chi_u(X) = \det(A - XI_n) = (a_1 - X)^{q_1} \cdots (a_k - X)^{q_k}$$ where $a_1, \ldots, a_k$ are the distinct eigenvalues and $q_i$ their algebraic multiplicities.
    
- **Cayley-Hamilton Theorem:** For any endomorphism $u \in \text{End}(E)$: $$\chi_u(u) = 0$$ Therefore, $\Pi_u \mid \chi_u$.
    
- **Eigenspace Decomposition:** $$E_i = \ker(u - a_i \text{Id}_E)^{q_i}$$ is called the characteristic subspace associated with eigenvalue $a_i$.
    

#### Section 4: Decomposition Theorems

- **Theorem (Primary Decomposition):** Let $E$ be a finite-dimensional $K$-vector space, $u \in \text{End}(E)$, and suppose the minimal polynomial factors as: $$\Pi_u(X) = (X - \lambda_1)^{r_1} \cdots (X - \lambda_k)^{r_k}$$ where $\lambda_1, \ldots, \lambda_k$ are distinct eigenvalues. Then:
    
    1. **Direct sum decomposition:** $$E = E_1 \oplus \cdots \oplus E_k$$ where $E_i = \ker(u - \lambda_i \text{Id}_E)^{r_i}$
        
    2. **Invariant subspaces:** Each $E_i$ is stable under $u$ (i.e., $u(E_i) \subseteq E_i$)
        
    3. **Restriction properties:** The restriction $u|_{E_i}$ has minimal polynomial $(X - \lambda_i)^{r_i}$
        
- **Relationship between polynomials:** $$\ker(\Pi_u(u)) = \ker(P_1(u)) \oplus \cdots \oplus \ker(P_r(u))$$ if $\Pi_u = P_1 \cdots P_r$ with $\gcd(P_i, P_j) = 1$ for $i \neq j$.
    

#### Section 5: Diagonalization and Trigonalization

- **Diagonalizability Criterion:** An endomorphism $u$ is diagonalizable if and only if its minimal polynomial splits into distinct linear factors: $$\Pi_u(X) = (X - \lambda_1) \cdots (X - \lambda_k)$$
    
    Equivalently: $u$ is diagonalizable $\Leftrightarrow$ $\chi_u$ splits and for all $i$, $\dim(\ker(u - \lambda_i \text{Id}_E)) = q_i$ (geometric multiplicity = algebraic multiplicity).
    
- **Trigonalizability Criterion:** An endomorphism $u$ is trigonalizable if and only if its characteristic polynomial splits completely over $K$: $$\chi_u(X) = (X - \lambda_1)^{q_1} \cdots (X - \lambda_k)^{q_k}$$ where all $\lambda_i \in K$.
    
- **Characteristic Subspace Dimensions:** For a trigonalizable endomorphism: $$\dim(E_i) = q_i$$ where $E_i = \ker(u - \lambda_i \text{Id}_E)^{q_i}$
    

---

## 📝 Notes

- The minimal polynomial is always a divisor of the characteristic polynomial: $\Pi_u \mid \chi_u$
- The degree of the minimal polynomial is at most the dimension of the space: $\deg(\Pi_u) \leq \dim(E)$
- For diagonalization, all eigenvalues must have geometric multiplicity equal to algebraic multiplicity
- The characteristic subspaces $E_i$ form a direct sum decomposition of $E$ when $u$ is trigonalizable
- Every polynomial that annihilates $u$ (i.e., $P(u) = 0$) is divisible by the minimal polynomial
- The minimal polynomial contains all eigenvalues of $u$ as roots
- Over $\mathbb{C}$, every endomorphism is trigonalizable (since every polynomial splits)
- An endomorphism is diagonalizable if and only if $E = \bigoplus_{i=1}^k \ker(u - \lambda_i \text{Id}_E)$
- The map $\Phi: K[X] \to \text{End}(E)$ given by $P \mapsto P(u)$ is a ring homomorphism
- Characteristic subspaces are stable under $u$ and the restriction of $u$ to each subspace has a particularly simple form