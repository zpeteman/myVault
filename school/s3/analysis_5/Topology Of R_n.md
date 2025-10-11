---
aliases:
  - Chapter_I
---

## 📚 Course Structure
- Section 1: $\mathbb{R}^n$ **Norms**
- Section 2:  **The various usual Norms of** $\mathbb{R}^n$
- Section 3: **Equivalent Norms**
- Section 4: **Open ball and closed ball**
- Section 5: **Open and Closed**
- Section 6: **Convergence of sequences in** $(\mathbb{R}^n, N)$

---
## 📐 Equations & Concepts

##### Norms:
- **(n=1) :** 
	if $x \in \mathbb{R}$ then the absolute value of it is noted :$$ |x| = Max(x,-x) $$
- **(n=2) :** 
	if $M(x,y)$ a point in the plan $\mathbb{R}^2$ of origin $O$, and the vector $\vec{u}$ and $u(x,y) \in \mathbb{R}$, we note : $$\left| \left| u \right| \right| = \sqrt{x^2 + y^2}$$
- **(n>2) :**
	we call **norm** of a number all function $f$ which is noted $\left| . \right|$ from $\mathbb{R}^2 \to \mathbb{R}^+$ and verifies the conditions: 
	- $\left| \left| u \right| \right| = 0 \iff u = 0, \forall u \in \mathbb{R}^n$.
	- $\left| \left| \alpha . u \right| \right| = \left| \left| \alpha \right| \right| . \left| \left| u \right| \right|, \forall \alpha \in \mathbb{R}, \forall u \in \mathbb{R}^n$.
	- **triangular inequality**.

#### type of Norms:
let $X = (x_1, \dots, x_n) \in \mathbb{R}^n$. we consider the applications:
- **The Norm** $N_1$ : $N_1 (X) = \sum_{i=1}^{i=n} \left|x_i\right|$.
- **The Euclidian Norm** $N_2$ : $N_2 (X) = \sum_{i=1}^{i=n} \left|x_i\right|^2$.
- **The Infinite Norm**: $N_{\infty}(X) = sup_{i=1,n} \left|x_i\right|$. 
#### Equivalent Norms:
we say that $N_1 , N_2$ are equivalent if there's $\alpha, \beta \in \mathbb{R}^+$ such that : $$\alpha N_1(X) \le N_2(X) \le \beta N_1(X)$$
#### Open ball and closed ball:
let $N \in \mathbb{R}^n$, let $a \in \mathbb{R}^n, r > 0$.
- **Open Ball :**
	. $$B(a,r) = \{x \in \mathbb{R}^n/N(a-x) < r\}$$
- **Closed Ball :** 
	.$$B(a,r) = \{x \in \mathbb{R}^n/N(a-x) \le r\}$$
#### Open and Closed:
let $O$ be a part of the normed space $(\mathbb{R}^n, N)$.
$O$ is **Opened** of $\mathbb{R}^n$ if $\forall x \in O$, there's $\epsilon > 0$ such that $B(x,\epsilon) \subset O$
- If $F \subset \mathbb{R}^n$, we say that $F$ is **Closed** in $\mathbb{R}^n$ if $F^c$ is **Opened** in $\mathbb{R}^n$.
where $F^c = \{x \in \mathbb{R}^n/x \notin R\}$. 

#### convergence of sequences in $(\mathbb{R}^n, N)$
Let $N$ be a norm on $\mathbb{R}^n$. Let $(X_m)_{m \in \mathbb{N}}$ be a sequence of vectors in $\mathbb{R}^n$. We say that $(X_m)$ converges to $L = (l_1, \dots, l_n) \in \mathbb{R}^n$ if for every $\varepsilon > 0$, there exists $N_\varepsilon \in \mathbb{N}$ such that: $$m \geq N_\varepsilon \;\;\Rightarrow\;\; N(X_m - L) \leq \varepsilon $$
We write: $$\lim_{m \to \infty} X_m = L$$
Let $(X_m)_{m \in \mathbb{N}}$ be a sequence of vectors in $\mathbb{R}^2$ where $X_m = (x_m,y_m)$ for all $m \in \mathbb{N}$.  
Then: $$\lim_{m \to \infty} X_m = L = (l_1, l_2) 
\;\;\Leftrightarrow\;\;
\left(\lim_{m \to \infty} x_m = l_1 \;\; \text{and} \;\; \lim_{m \to \infty} y_m = l_2 \right)$$
---

## 📝 Notes
- **triangular inequality :** $\left|x + y\right| \le \left| x \right| + \left| y \right|, \forall x,y \in \mathbb{R}^n$.
- we say that the **norm** of $u$ is Euclidian, if $\left| \left| u \right| \right|$ if defined from $\mathbb{R}^2 \to \mathbb{R}^+$.
- if $N$ is a norm in $\mathbb{R}^n$. then $\forall x, y \in \mathbb{R}^n$ we have: $\left|N(x) - N(y)\right| \le N(x-y)$.
- the **usual Norms of** $\mathbb{R}^n$ are **equivalent**.  
- In $\mathbb{R}^n$ all the **Norms** are **equivalent**.
- the **intersection** of a **finite number of Opened** is an **Opened**.
- All **unions** of **opened** is **Opened**.
- The notion of **convergence of sequences** does **not depend** on **the chosen norm**.