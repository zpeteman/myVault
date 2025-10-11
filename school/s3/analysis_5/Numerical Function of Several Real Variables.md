---
aliases:
  - chapter_II
---
## 📚 Course Structure
- Section 1: **Introduction**.
- Section 2: **Limit and Continuity**.

---
## 📐 Equations & Concepts
## Introduction:
A numerical function of $n$ real variables is a mapping $f$ from $D \subset \mathbb{R}^n$ to $\mathbb{R}$. 
$D$ is called the domain of definition of $f$ and is denoted $D_f$.

#### Limit and Continuity:
- **limit:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$, defined on a neighborhood $V$ of $x_0 \in \mathbb{R}^n$, except possibly at $x_0$, and let $l \in \mathbb{R}$. We say that $f$ tends to $l$ as $x$ tends to $x_0$ if, for every $\varepsilon > 0$, there exists $\eta > 0$ such that $$ |f(x) - l| < \varepsilon, \quad \forall x \in B(x_0, \eta) \cap V \setminus \{x_0\} $$
	where $B(x_0, \eta)$ is defined using any norm on $\mathbb{R}^n$. We write: $$ l = \lim_{x \to x_0} f(x) $$
- **Continuity:**
	Let $f$ be a function from $D \subset \mathbb{R}^n$ to $\mathbb{R}$ and $x_0 \in D$ with $D$ a neighborhood of $x_0$. We say that $f$ is **continuous** at $x_0$ if: $$\lim_{x \to x_0} f(x) = f(x_0) $$
- **Partial Mappings:**
	Let $f$ be a function from $\mathbb{R}^n$ to $\mathbb{R}$, defined on a neighborhood of the point $a = (a_1, \ldots, a_n) \in \mathbb{R}^n$. For each $i = 1, \ldots, n$, define the function $\varphi_i$ from $\mathbb{R}$ to $\mathbb{R}$ by: $$\varphi_i(t) = f(a_1, \ldots, a_{i-1}, t, a_{i+1}, \ldots, a_n), \quad \forall t \in \mathbb{R} $$ The function $\varphi_i$ is called the $i$-th **partial mapping** of $f$ relative to $a$.


---
## 📝 Notes
- A function is defined in a neighborhood of $x \in \mathbb{R}^n$ if there exists $r > 0$ such that $f(y)$ exists for all $y \in B(x, r)$ (except possibly at $x$ itself), where $B(x, r)$ is the open ball of radius $r$ centered at $x$.
- $\forall \varepsilon > 0, \exists \eta > 0$ such that: $|x - x_0| < \eta \implies |f(x) - l| < \varepsilon$
	As with single-variable functions, we generalize this notion to $l = \infty$ and $l = -\infty$.
- If $f$ is **continuous** at $a$, then $\varphi_i$ is continuous at $a_i$ for all $i = 1, \ldots, n$.	