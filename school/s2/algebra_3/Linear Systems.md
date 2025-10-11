---
aliases:
  - chapter_III
---

## 📚 Course Structure
- Section 1: **Linear Systems: Definitions & Types**
- Section 2: **Solving Linear Systems (Gauss & Cramer)**
- Section 3: **General Case: Non-square & Singular Matrices**

---
## 📐 Equations & Concepts
#### Linear Systems: Definitions & Types
- **Linear System:** $m$ equations, $n$ unknowns $x_1, ..., x_n$:
  $$
  \begin{cases}
    a_{11}x_1 + a_{12}x_2 + ... + a_{1n}x_n = b_1 \\
    a_{21}x_1 + a_{22}x_2 + ... + a_{2n}x_n = b_2 \\
    \vdots \\
    a_{m1}x_1 + a_{m2}x_2 + ... + a_{mn}x_n = b_m
  \end{cases}
  $$
  - Matrix form: $AX = B$
  - **Homogeneous system:** $AX = 0$
  - **Compatible:** At least one solution
  - Solutions: None, unique, or infinite

#### Solving Linear Systems (Gauss & Cramer)
- **Gauss Method:**
  - Use row operations to simplify the system
  - Operations: swap rows, multiply a row by nonzero constant, add multiples of rows
  - Example: Reduce to upper triangular, then back-substitute
- **Cramer System:**
  - Square ($n \times n$) and invertible matrix ($\det A \neq 0$)
  - Unique solution: $X = A^{-1}B$
  - **Cramer's Rule:**
    - For each unknown $x_i$, replace $i$-th column of $A$ with $B$ to get $A_i$
    - $x_i = \dfrac{\det A_i}{\det A}$

#### General Case: Non-square & Singular Matrices
- **Non-square or $\det A = 0$:**
  - Extract largest invertible submatrix (Cramer subsystem)
  - Solve subsystem for partial solution
  - Substitute back to check if it solves the full system
  - If not, no solution; if yes, parametric solution (infinite solutions)

---
## 📝 Notes
- A linear system can have no solution, one solution, or infinitely many solutions.
- Gauss method uses row operations to simplify and solve systems.
- Cramer's rule applies only to square, invertible systems.
- For non-square or singular systems, solve the largest Cramer subsystem and check consistency.
- Solutions may be parametric if there are free variables.
