---
aliases:
  - chapter_II
---

## 📚 Course Structure
- Section 1: **Matrices and Operations**
- Section 2: **Matrices and Linear Maps**
- Section 3: **Determinants and Applications**

---
## 📐 Equations & Concepts
#### Matrices and Operations:
- **Definition:**
  A matrix $A$ with $m$ rows and $n$ columns over a field $K$ ($\mathbb{R}$ or $\mathbb{C}$) is written as $A = (a_{ij})$ with $1 \leq i \leq m$, $1 \leq j \leq n$.
  - The set of all $m \times n$ matrices over $K$ is $M_{m,n}(K)$.
  - **Transpose:** $^tA = (a_{ji})$ in $M_{n,m}(K)$.
  - **Identity matrix:** $I_n$ has $a_{ii} = 1$, $a_{ij} = 0$ for $i \neq j$.
  - **Diagonal matrix:** $a_{ii} = d_i$, $a_{ij} = 0$ for $i \neq j$.
  - **Lower triangular:** $a_{ij} = 0$ for $i < j$.
- **Vector Space Structure:**
  - $M_{m,n}(K)$ is a vector space of dimension $mn$.
  - Example: A basis for $M_{2,3}(\mathbb{R})$ is the set of matrices with a single 1 and the rest 0.
- **Matrix Addition and Scalar Multiplication:**
  - Usual entrywise operations.
- **Matrix Multiplication:**
  - Defined when the number of columns of the first equals the number of rows of the second.
- **Binomial Formula:**
  - If $A, B \in M_n(K)$ and $AB = BA$, then $(A+B)^p = \sum_{k=0}^p C_p^k A^k B^{p-k}$.

#### Matrices and Linear Maps:
- **Associated Matrix:**
  - For $f: E \to E'$ linear, with bases $B$ and $B'$, the matrix $M_f^{B,B'}$ has columns given by the coordinates of $f(e_1), ..., f(e_n)$ in $B'$.
  - The matrix depends on the choice of bases.
- **Matrix of a Linear Map:**
  - If $f: E \to F$ and $g: F \to G$, then $M_{g \circ f} = M_g M_f$ (with respect to appropriate bases).
  - $f$ is bijective $\iff$ $M_f$ is invertible.
- **Matrix Representation:**
  - Any vector $x$ in $E$ can be written as a column matrix $X$ of its coordinates.
  - $f(x)$ corresponds to $Y = AX$ where $A$ is the matrix of $f$.
- **Change of Basis:**
  - The change of basis matrix $P$ from $B$ to $B'$ has columns as coordinates of $B'$ vectors in $B$.
  - $X' = PX$ relates coordinates in different bases.
  - For a linear map, $A' = Q^{-1} A P$ gives the new matrix under basis changes.

#### Determinants and Applications:
- **Determinant:**
  - For $A \in M_n(K)$, $\det(A)$ is defined recursively by expansion along a row or column.
  - $n=2$: $\det\begin{pmatrix}a & b \\ c & d\end{pmatrix} = ad - bc$
  - $n=3$: Use Sarrus' rule or cofactor expansion.
- **Properties:**
  - $\det(AB) = \det(A)\det(B)$
  - $\det(^tA) = \det(A)$
  - If two rows or columns are equal or colinear, $\det(A) = 0$.
- **Cofactors and Inverse:**
  - The cofactor $C_{ij} = (-1)^{i+j} \det(A_{ij})$ where $A_{ij}$ is $A$ with row $i$ and column $j$ removed.
  - $A^{-1} = \frac{1}{\det(A)}\,^t\!\text{Com}(A)$ if $\det(A) \neq 0$.
- **Gauss Pivot Method:**
  - To find $A^{-1}$, augment $A$ with $I_n$ and use row operations to reduce $A$ to $I_n$; the transformed $I_n$ becomes $A^{-1}$.

---
## 📝 Notes
- Matrices generalize arrays of numbers and represent linear maps.
- The matrix of a linear map depends on the choice of bases.
- The determinant gives information about invertibility and volume scaling.
- The inverse of a matrix can be found by cofactors or by row reduction (Gauss method).
- Changing bases transforms both vectors and matrices via invertible matrices.
