---
aliases:
  - Chapter_I
---

## 📚 Course Structure
- Section 1: **Series in a Normed Vector Space**
- Section 2: **Series with Positive Terms**

---

## 📐 Equations & Concepts
#### Series in a Normed Vector Space
- **Definition**
	- Let $(u_n)_{n \in \mathbb{N}} \in E^\mathbb{N}$, the series $\sum_n u_n$ is the sequence $(S_n)_{n \in \mathbb{N}}$ defined by:$$S_n = \sum_{k=0}^n u_k$$
	- $S_n$ is the **partial sum of order $n$**.
-  **Series Convergence**
	- The series $\sum_n u_n$ **converges** if $(S_n)$ converges.
	- If $\lim S_n = S$, we write $S = \sum_{n=0}^{+\infty} u_n$.
	- The **remainder of order $n$** is: $$R_n = \sum_{k=n+1}^{+\infty} u_k$$
- **Necessary Condition for Convergence**
	- If $\sum u_n$ converges, then $\lim u_n = 0$.
	- The converse is false (e.g., harmonic series).
- **Cauchy Criterion** 
	- The series $\sum u_n$ is Cauchy if: $$ \forall \varepsilon > 0, \exists N, \forall q \geq p \geq N, \quad \left\| \sum_{n=p}^q u_n \right\| \leq \varepsilon$$
- **Absolute Convergence**
	- $\sum u_n$ is **absolutely convergent** if $\sum \|u_n\|$ converges.
	- In a complete space, every absolutely convergent series is convergent.

#### Series with Positive Terms 
$\sum u_n$ has positive terms if $\forall n, u_n \geq 0$.
- **criteria of monotonicity:**
	A series with positive real terms $\sum_n u_n$ converges if and only if the associated sequence $(S_n)_{n\in\mathbb{N}}$ is bounded above, and in this case, the sum of the series is the least upper bound (supremum) of the associated sequence.
- **Comparison Criterion:**
	- We say that $u_n = o(v_n)$ if there exists $M > 0$ such that for all $n$, $u_n \leq M v_n$.
	- Let $\sum_n u_n$ and $\sum_n v_n$ be two series with positive terms such that for all $n \in \mathbb{N}$, $u_n = o(v_n)$. Then: 
		1. If $\sum_n v_n$ converges $\Rightarrow \sum_n u_n$ converges. 
		2. If $\sum_n u_n$ diverges $\Rightarrow \sum_n v_n$ diverges.
	- Let $\sum_n u_n$ and $\sum_n v_n$ be two series with positive terms such that $$\lim_{n \to +\infty} \frac{u_n}{v_n} = k$$ 
		1. If $k$ is a finite nonzero number, then $\sum_n u_n$ and $\sum_n v_n$ have the same behavior (both converge or both diverge). 
		2. If $k = 0$ and $\sum_n v_n$ converges, then $\sum_n u_n$ converges. 
		3. If $k = +\infty$ and $\sum_n v_n$ diverges, then $\sum_n u_n$ diverges.
	- **Power Test Rule:**
		Let $\sum_n u_n$ be a series with positive terms and let $\alpha \in \mathbb{R}$ such that $$ \lim_{n \to +\infty} n^\alpha u_n = k. $$
		1. If $k$ is a nonzero finite number and $\alpha > 1$, then $\sum_n u_n$ converges. 
		2. If $k$ is a nonzero finite number and $\alpha \leq 1$, then $\sum_n u_n$ diverges. 
		3. If $k = 0$ and $\alpha > 1$, then $\sum_n u_n$ converges. 
		4. If $k = +\infty$ and $\alpha \leq 1$, then $\sum_n u_n$ diverges.
- **Comparison Criterion Between a Series and Its Integral:**
	Let $f: \mathbb{R}^+ \to \mathbb{R}^+$ be a continuous and decreasing function.
	1. $\sum_n f(n)$ converges if and only if $$\int_0^{+\infty} f(x)\,dx$$ converges. 
	2. For all $k \in \mathbb{N}$, $$ \int_{k+1}^{+\infty} f(x)\,dx \leq \sum_{n \geq k+1} f(n) \leq \int_k^{+\infty} f(x)\,dx. $$
- **Indirect Comparison Criterion:**
	Let $\sum u_n$ and $\sum v_n$ be two series with positive terms. If $\frac{u_{n+1}}{u_n} \leq \frac{v_{n+1}}{v_n}$ and $\sum v_n$ converges, then $\sum u_n$ converges.
- **d'Alembert's Criterion:**
	- Let  be a series with positive terms. 
		1. If there exists $q > 0$ such that $\frac{u_{n+1}}{u_n} \leq q < 1$, $\forall n \in \mathbb{N}$, then $\sum u_n$ converges. 
		2. If there exists $q > 0$ such that $\frac{u_{n+1}}{u_n} \geq q \geq 1$, $\forall n \in \mathbb{N}$, then $\sum u_n$ diverges.
	- **Corollary:** 
		Let $\sum u_n$ be a series with positive terms such that $$ \lim_{n \to +\infty} \frac{u_{n+1}}{u_n} = k. $$
		1. If $k < 1$, then $\sum u_n$ converges. 
		2. If $k > 1$, then $\sum u_n$ diverges. 
		3. If $k = 1$, then nothing can be concluded about the nature of the series $\sum u_n$.
- **Raab-Duhamel Criterion:**
	Let $\sum u_n$ be a series with positive terms. 
	1. If there exists $q > 0$ such that $n\left(\frac{u_n}{u_{n+1}} - 1\right) \geq q \geq 1$ for all $n \in \mathbb{N}^*$, then $\sum u_n$ converges. 
	2. If there exists $q > 0$ such that $n\left(\frac{u_n}{u_{n+1}} - 1\right) \leq q < 1$ for all $n \in \mathbb{N}^*$, then $\sum u_n$ diverges.

---

## 📝 Notes
- A **series** can be **convergent** without being **absolutely convergent**.
- The **nature** of a **series** doesn't change by **truncation**.
- The **set of convergent series** forms a **vector subspace of $S(E)$**.
- For **linear continuous** maps: if $\sum u_n$ converges, then $\sum f(u_n)$ converges to $f(\sum u_n)$.