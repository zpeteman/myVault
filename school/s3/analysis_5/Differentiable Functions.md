---
aliases:
  - chapter_III
---
## 📚 Course Structure
 - Section 1: **Differential**.
 - Section 2: **Partial Derivative**.
 - Section 3: **Function from $\mathbb{R}^n$ to $\mathbb{R}^p$**. 
 - Section 4: **Operations on Differentiable Numerical Functions**.
 - Section 5: **Geometric Interpretation of Differentiability**.
 - Section 6: **Higher-order Partial Derivative**.
 - Section 7: **Schwarz's Theorem**.
 - Section 8: **Mean Value Formula and Taylor's Formula**.
 - Section 9: **Extremum Conditions**.

---
## 📐 Equations & Concepts
#### Differential:
- **Definition:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$, defined in a neighborhood $V$ of a point $x \in \mathbb{R}^n$. We say that $f$ is $\textbf{differentiable}$ at the point $x$ if there exists a (unique) linear map, which we denote by $df_x$, from $\mathbb{R}^n$ to $\mathbb{R}$, and a function $\varepsilon$ from $\mathbb{R}^n$ to $\mathbb{R}$ such that: for every $h \in \mathbb{R}^n$ with $x + h \in V$, we have: $$ f(x + h) = f(x) + df_x(h) + \|h\| \varepsilon(h) $$ where $\lim_{h \to 0} \varepsilon(h) = 0$. $df_x$ is called the $\textbf{differential map}$ of the function $f$ at the point $x$; $df_x \in \mathcal{L}(\mathbb{R}^n, \mathbb{R})$.
- **Uniqueness of the Differential:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$ and $x \in \mathbb{R}^n$. If $f$ is differentiable at the point $x$, then  is unique.
- **Proposition:**
	Let $f : \mathbb{R}^n \to \mathbb{R}$, $x \in \mathbb{R}^n$. $f$ is differentiable at $x$ if and only if there exist $(A_1, ..., A_n) \in \mathbb{R}^n$ and $n$ functions $\varepsilon_i : \mathbb{R}^n \to \mathbb{R}$ such that, for all $h \to (h_1, ..., h_n)$ small enough, we have: $$ f(x + h) = f(x) + \sum_{i=1}^n A_i h_i + \sum_{i=1}^n h_i \varepsilon_i(h) $$ with $\lim_{h \to 0} \varepsilon_i(h) = 0$, $\forall i = 1, ..., n$

#### Partial Derivative:
- **Definition:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$, differentiable at the point $x = (x_1, \ldots, x_n)$. Let $\varphi_i$ be the $i$-th partial map from $\mathbb{R}$ to $\mathbb{R}$, being the $i$-th partial application of $f$ relative to $x$, for $i = 1, \ldots, n$.
- **Theorem:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$, defined in a neighborhood $V$ of a vector $x \in \mathbb{R}^n$. If $f$ admits continuous partial derivatives at $x$, then $f$ is differentiable at $x$. We say $f$ is of class $C^1$ at $x$.
- **Directional Derivative:**
	Let $f$ be a function defined in a neighborhood of $x \in \mathbb{R}^n$ and $u$ a unit vector ($\|u\| = 1$). 
	The directional derivative of $f$ at $x$ in the direction $u$ is the limit, when it exists, of the ratio $(f(x + \lambda u) - f(x)) / \lambda$ as $\lambda$ tends to zero. Denoted as: $$ D_u f(x) = \lim_{\lambda \to 0} \frac{f(x + \lambda u) - f(x)}{\lambda} $$

#### Function from $\mathbb{R}^n$ to $\mathbb{R}^p$
- **Definition:**
	Let $D \subset \mathbb{R}^n$ (an open set) and $f : D \rightarrow \mathbb{R}^p$ defined on a neighborhood $V$ of a point $x \in D$, $x = (x_1, x_2, ..., x_n)$. $f$ is said to be differentiable at $x$ if there exists a linear map $df_x : \mathbb{R}^n \rightarrow \mathbb{R}^p$, that is, there exists a mapping $\varepsilon : \mathbb{R}^n \rightarrow \mathbb{R}^p$ with $\lim_{h \to 0} \varepsilon(h) = 0$ such that for every $h \in \mathbb{R}^n$ with $x + h \in V$, we have: $$ f(x + h) - f(x) = df_x(h) + \|h\|\varepsilon(h) $$ $f$ is differentiable on $D$ if it is differentiable at every point of $D$.
- **Proposition:**
	Let $f : \mathbb{R}^n \rightarrow \mathbb{R}^p$ be defined in a neighborhood of $x$ in $\mathbb{R}^n$. The following statements are equivalent: 
	1. $f$ is differentiable at $x$. 
	2. Each component $P_i \circ f = f_i$ is differentiable at $x$, for all $i = 1, ..., n$, where $P_i$ is the $i$-th projection.
- **Jacobian matrix:**
	The matrix associated to $df_x$ is called the Jacobian matrix of $f$ at the point $x$ and is denoted: $$ M(df_x) := J_{f(x)} $$
- **theorem:**
	Let $f : \mathbb{R}^n \rightarrow \mathbb{R}^p$ be differentiable at $x$ in $\mathbb{R}^n$ and $g : \mathbb{R}^p \rightarrow \mathbb{R}^q$ differentiable at $f(x) \in \mathbb{R}^p$. Then $g \circ f$ is differentiable at $x$ and $d(g \circ f)_x = dg_{f(x)} \circ df_x$. $$ J_{g \circ f(x)} = J_{g(f(x))} J_{f(x)} $$

#### Operations on Differentiable Numerical Functions
Let $f$ and $g$ be two numerical functions on $\mathbb{R}^n$ differentiable at the point $x \in \mathbb{R}^n$. 
1. $\lambda f$ is differentiable at $x$ and $d(\lambda f)_x = \lambda d f_x$, where $\lambda \in \mathbb{R}$. 
2. $f + g$ is differentiable at $x$ and $d(f + g)_x = d f_x + d g_x$. 
3. $fg$ is differentiable at $x$ and $d(fg)_x = g(x) d f_x + f(x) d g_x$. 
4. If $g(x) \neq 0$, then $\frac{f}{g}$ is differentiable at $x$ and $$ d\left(\frac{f}{g}\right)_x = \frac{g(x) d f_x - f(x) d g_x}{(g(x))^2} $$
#### Geometric Interpretation of Differentiability
Two functions $f$ and $g$ from $\mathbb{R}^n$ to $\mathbb{R}^p$ are said to be tangent at a point $x_0 \in \mathbb{R}^n$ if $$ \lim_{x \to x_0} \frac{\|f(x) - g(x)\|}{\|x - x_0\|} = 0. $$ i.e. $$ f(x) - g(x) = \|x - x_0\| \varepsilon(x - x_0), \quad \text{where} \quad \lim_{h \to 0} \varepsilon(h) = 0. $$

#### Higher-order Partial Derivative
Let $U$ be an open subset of  and $f : U \rightarrow \mathbb{R}$ differentiable on $U$ ($\forall i = 1, \ldots, n$, $\frac{\partial f}{\partial x_i} : U \rightarrow \mathbb{R}$ is well defined, since $df_x : U \rightarrow L(\mathbb{R}^n, \mathbb{R})$).
Let $i, j = 1, \ldots, n$. If the function $\frac{\partial f}{\partial x_i} : U \rightarrow \mathbb{R}$ is differentiable with respect to $x_j$, then its derivative is denoted: $$ \frac{\partial}{\partial x_j} \frac{\partial f}{\partial x_i}(x) = \frac{\partial^2 f}{\partial x_j \partial x_i}(x) $$

#### Schwarz's Theorem:
- **Schwarz's Theorem:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$ of class $C^1$ on an open subset $U$ of $\mathbb{R}^n$ and admitting continuous second-order partial derivatives at the point $x_0 \in U$: $$ \frac{\partial^2 f}{\partial x_i \partial x_j} \quad \text{and} \quad \frac{\partial^2 f}{\partial x_j \partial x_i} $$ Then: $$ \frac{\partial^2 f}{\partial x_i \partial x_j}(x_0) = \frac{\partial^2 f}{\partial x_j \partial x_i}(x_0) $$
- **Converse:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$ defined in a neighborhood $U$ of a vector $x_0 \in \mathbb{R}^n$. $f$ is of class $C^1$ at $x_0$ (admits continuous partial derivatives at $x_0$) if and only if: 
	1. $f$ is differentiable at $x_0$, and 
	2. the map $df : U \rightarrow L(\mathbb{R}^n, \mathbb{R})$ is continuous at $x_0$.

### Mean Value Formula and Taylor's Formula:
- **Mean Value Theorem:**
	Let $D$ be a convex subset of $\mathbb{R}^n$ and $f : D \to \mathbb{R}$ differentiable on $D$. If $x, x + h \in D$, there exists $\theta \in (0, 1)$ such that: $$ f(x + h) - f(x) = df_{x + \theta h}(h) $$
- **Taylor series:**
	Let $f : \mathbb{R}^n \to \mathbb{R}$ be of class $C^2$ in a neighborhood of $a \in \mathbb{R}^n$. For $x$ near $a$: $$ f(x) \approx f(a) + df_a(x - a) + \frac{1}{2} D^2f_a(x - a, x - a) $$ where: 
	- $df_a$ is the differential of $f$ at $a$ (the gradient, noted $\nabla f(a)$, so $df_a(h) = \nabla f(a) \cdot h$) 
	- $D^2f_a$ is the second differential (the Hessian), so $D^2f_a(h, h) = h^T H_f(a) h$ 
	**Expanded:** $$ f(x) \approx f(a) + \nabla f(a) \cdot (x - a) + \frac{1}{2}(x - a)^T H_f(a) (x - a) $$ where $H_f(a)$ is the Hessian matrix of $f$ at $a$.

#### Extremum Conditions:
- **Critical Points:** 
	Let $f : \mathbb{R}^n \to \mathbb{R}$ be of class $C^2$. A point $a \in \mathbb{R}^n$ is called a **critical point** of  if: $$ \nabla f(a) = 0 $$
- **Second-Order Condition (Hessian Test):** 
	Let $H_f(a)$ denote the Hessian matrix of  at $a$ ($n \times n$ matrix of second partial derivatives). 
	- If $H_f(a)$ is **positive definite**, then $a$ is a **local minimum**. 
	- If $H_f(a)$ is **negative definite**, then $a$ is a **local maximum**. 
	- If $H_f(a)$ is **indefinite** (has both positive and negative.
- **Sufficient Condition: Taylor Expansion:** 
	For  near a critical point $a$: $$ f(x) \approx f(a) + \frac{1}{2} (x - a)^T H_f(a) (x - a) $$ where $H_f(a)$ is the Hessian matrix at $a$.

---
## 📝 Notes
- The matrix of the linear map $df_x$ is a row vector of the form $M(df_x) = (l_1, l_2, ..., l_n) \quad \text{where} \quad l_i \in \mathbb{R}$ If $h = (h_1, ..., h_n) \in \mathbb{R}^n$, then $df_x.h = \sum_{i=1}^n l_i h_i$.
- **Differentiability** does not depend on the choice of **norm**.
- $D$ be an open subset of $\mathbb{R}^n$. $f$ is said to be differentiable on $D$ if $f$ is differentiable at every point of $D$.
- Differentiability $\Rightarrow$ continuity.
- Every linear map is continuous.
- If $f$ is differentiable at $x$, then $\varphi_i$ is differentiable at $x_i$ for all $i = 1, \ldots, n$.
- Continuous partial derivatives means that for every $i \in \{1, \ldots, n\}$, the map $\frac{\partial f}{\partial x_i} : y \mapsto \frac{\partial f}{\partial x_i}(y)$ is continuous at $x$.
- for $u = e_i$, the $i$-th canonical basis vector of $\mathbb{R}^n$: $$ D_{e_i} f(x) = \lim_{\lambda \to 0} \frac{f(x + \lambda e_i) - f(x)}{\lambda} = \frac{\partial f}{\partial x_i}(x) $$
- If $f$ is differentiable at $x \in \mathbb{R}^n$, then $f$ has partial derivatives at $x$ in all directions.