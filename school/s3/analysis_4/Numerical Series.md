---
aliases:
  - Chapter_I
---
## 📚 Course Structure

- Section 1: **Series in a Normed Vector Space**
- Section 2: **Series with Positive Terms**
- Section 3: **Series with Any Terms**
- Section 4: **Product Series**

---

## 📐 Equations & Concepts

### Series in a Normed Vector Space
- **Definition**
	- Let $(u_n)_{n \in \mathbb{N}} \in E^\mathbb{N}$, the series $\sum_n u_n$ is the sequence $(S_n)_{n \in \mathbb{N}}$ defined by:$$S_n = \sum_{k=0}^n u_k$$
	- $S_n$ is the **partial sum of order $n$**.
- **Series Convergence**
	- The series $\sum_n u_n$ **converges** if $(S_n)$ converges.
	- If $\lim S_n = S$, we write $S = \sum_{n=0}^{+\infty} u_n$.
	- The **remainder of order $n$** is: $$R_n = \sum_{k=n+1}^{+\infty} u_k$$
- **Necessary Condition for Convergence**
	- If $\sum u_n$ converges, then $\lim u_n = 0$.
	- The converse is false (e.g., harmonic series).
- **Cauchy Criterion**
	- The series $\sum u_n$ is Cauchy if: $$ \forall \varepsilon > 0, \exists N, \forall q \geq p \geq N, \quad \left| \sum_{n=p}^q u_n \right| \leq \varepsilon$$
- **Absolute Convergence**
	- $\sum u_n$ is **absolutely convergent** if $\sum |u_n|$ converges.
	- In a complete space, every absolutely convergent series is convergent.

### Series with Positive Terms
	$\sum u_n$ has positive terms if $\forall n, u_n \geq 0$.
- **Criteria of Monotonicity**
	A series with positive real terms $\sum_n u_n$ converges if and only if the associated sequence $(S_n)_{n\in\mathbb{N}}$ is bounded above, and in this case, the sum of the series is the least upper bound (supremum) of the associated sequence.
- **Comparison Criterion**
	- We say that $u_n = o(v_n)$ if there exists $M > 0$ such that for all $n$, $u_n \leq M v_n$.
	- Let $\sum_n u_n$ and $\sum_n v_n$ be two series with positive terms such that for all $n \in \mathbb{N}$, $u_n = o(v_n)$. Then:
	    1. If $\sum_n v_n$ converges $\Rightarrow \sum_n u_n$ converges.
	    2. If $\sum_n u_n$ diverges $\Rightarrow \sum_n v_n$ diverges.
	- Let $\sum_n u_n$ and $\sum_n v_n$ be two series with positive terms such that $$\lim_{n \to +\infty} \frac{u_n}{v_n} = k$$
	    1. If $k$ is a finite nonzero number, then $\sum_n u_n$ and $\sum_n v_n$ have the same behavior (both converge or both diverge).
	    2. If $k = 0$ and $\sum_n v_n$ converges, then $\sum_n u_n$ converges.
	    3. If $k = +\infty$ and $\sum_n v_n$ diverges, then $\sum_n u_n$ diverges.
- **Power Test Rule**
	Let $\sum_n u_n$ be a series with positive terms and let $\alpha \in \mathbb{R}$ such that $$ \lim_{n \to +\infty} n^\alpha u_n = k. $$
	1. If $k$ is a nonzero finite number and $\alpha > 1$, then $\sum_n u_n$ converges.
	2. If $k$ is a nonzero finite number and $\alpha \leq 1$, then $\sum_n u_n$ diverges.
	3. If $k = 0$ and $\alpha > 1$, then $\sum_n u_n$ converges.
	4. If $k = +\infty$ and $\alpha \leq 1$, then $\sum_n u_n$ diverges.
- **Comparison Criterion Between a Series and Its Integral**
	Let $f: \mathbb{R}^+ \to \mathbb{R}^+$ be a continuous and decreasing function.
	1. $\sum_n f(n)$ converges if and only if $$\int_0^{+\infty} f(x),dx$$ converges.
	2. For all $k \in \mathbb{N}$, $$ \int_{k+1}^{+\infty} f(x),dx \leq \sum_{n \geq k+1} f(n) \leq \int_k^{+\infty} f(x),dx. $$
- **Indirect Comparison Criterion**
	Let $\sum u_n$ and $\sum v_n$ be two series with positive terms. If $\frac{u_{n+1}}{u_n} \leq \frac{v_{n+1}}{v_n}$ and $\sum v_n$ converges, then $\sum u_n$ converges.
- **d'Alembert's Criterion (Ratio Test)**
	Let $\sum u_n$ be a series with positive terms such that $$ \lim_{n \to +\infty} \frac{u_{n+1}}{u_n} = k. $$
	    1. If $k < 1$, then $\sum u_n$ converges.
	    2. If $k > 1$, then $\sum u_n$ diverges.
	    3. If $k = 1$, then nothing can be concluded about the nature of the series $\sum u_n$.
- **Raab-Duhamel Criterion**
	Let $\sum_n u_n$ be a series with positive terms such that $$\lim_{n \to +\infty} n\left(\frac{u_n}{u_{n+1}} - 1\right) = k.$$
	1. If $k > 1$, then $\sum_n u_n$ converges.
	2. If $k < 1$, then $\sum_n u_n$ diverges.
	3. If $k = 1$, nothing can be concluded about the nature of the series $\sum_n u_n$.
- **Gauss Criterion**
	Let $\sum_{n \geq 1} u_n$ be a series with positive terms such that $$\frac{u_n}{u_{n+1}} = \lambda + \frac{\mu}{n} + \frac{c_n}{n^2} \quad \text{or} \quad \frac{u_n}{u_{n+1}} = \lambda + \frac{\mu}{n} + o\left(\frac{1}{n^2}\right)$$ where $(c_n)_n$ is a bounded sequence.
	1. If $\lambda > 1$, then $\sum_{n \geq 1} u_n$ converges, for all $\mu$.
	2. If $\lambda < 1$, then $\sum_{n \geq 1} u_n$ diverges, for all $\mu$.
	3. If $\lambda = 1$, we distinguish two cases:
	    - a) If $\mu \leq 1$, then $\sum_{n \geq 1} u_n$ diverges.
	    - b) If $\mu > 1$, then $\sum_{n \geq 1} u_n$ converges.
- **Cauchy Criterion (Root Test)**
	Let $\sum_n u_n$ be a series with positive terms such that $$\lim_{n \to +\infty} \sqrt[n]{u_n} = k.$$
	1. If $k < 1$, then $\sum_n u_n$ converges.
	2. If $k > 1$, then $\sum_n u_n$ diverges.
	3. If $k = 1$, nothing can be concluded about the nature of the series $\sum_n u_n$.
- **Logarithm Criterion**
	Let $\sum_n u_n$ be a series with positive terms such that $$\lim_{n \to +\infty} \frac{\ln \frac{1}{u_n}}{\ln n} = k.$$
	1. If $k > 1$, then $\sum_n u_n$ converges.
	2. If $k < 1$, then $\sum_n u_n$ diverges.
	3. If $k = 1$, nothing can be concluded about the nature of the series $\sum_n u_n$.
### Series with Any Terms
- **Definition**
	Let $(u_n)_{n \in \mathbb{N}}$ be a sequence with real terms of any sign or complex terms. We say that the series $\sum_n u_n$ is **absolutely convergent** if and only if $\sum_n |u_n|$ converges, where $|u_n|$ denotes either the absolute value of $u_n$ if $u_n \in \mathbb{R}$ or the modulus of $u_n$ if $u_n \in \mathbb{C}$.
- **Dirichlet or Abel Criterion**
	- Let $(v_n)_{n \in \mathbb{N}}$ be a sequence with positive terms, decreasing, such that $\lim_{n \to +\infty} v_n = 0$, then the series $\sum_n v_n Z^n$ converges if $|Z| = 1$ and $Z \neq 1$.
	- Let $(v_n)_{n \in \mathbb{N}}$ be a sequence with positive terms, decreasing, such that $\lim_{n \to +\infty} v_n = 0$, then the series $\sum_n v_n e^{in\theta}$ converges for $\theta \neq 2k\pi$.
	- Let $(v_n)_{n \in \mathbb{N}}$ be a sequence with positive terms, decreasing, such that $\lim_{n \to +\infty} v_n = 0$, then the series $\sum_n v_n \cos n\theta$ and $\sum_n v_n \sin n\theta$ converge for $\theta \neq 2k\pi$.
- **Alternating Series**
	We say that $\sum_n u_n$ is an alternating series if $u_n = (-1)^n v_n$ where $v_n$ is a sequence with positive terms.
	**Leibniz Theorem:** 
		Let $(v_n)_{n \in \mathbb{N}}$ be a sequence with positive terms, decreasing, that converges to 0. Then the series $\sum_n (-1)^n v_n$ converges. Moreover, we have: $$\left|\sum_{k=n+1}^{+\infty} (-1)^k v_k\right| \leq v_{n+1}$$
### Product Series
- **Definition:** 
	Let $u_n$ and $v_n$ be two series. The series $$\sum_n w_n = \sum_n u_n \cdot \sum_n v_n$$ is called the **product series** of the series $\sum_n u_n$ and $\sum_n v_n$, where $$w_n = \sum_{k=0}^n u_k v_{n-k}$$
- **Theorem:** 
	If the two series $\sum_n u_n$ and $\sum_n v_n$ are absolutely convergent, then the product series is absolutely convergent and has as its sum the product of the two sums: $$\sum_{n=0}^\infty w_n = \left(\sum_{n=0}^\infty u_n\right)\left(\sum_{n=0}^\infty v_n\right)$$

---

## 📝 Notes

- A **series** can be **convergent** without being **absolutely convergent**.
- The **nature** of a **series** doesn't change by **truncation**.
- The **set of convergent series** forms a **vector subspace of $S(E)$**.
- For **linear continuous** maps: if $\sum u_n$ converges, then $\sum f(u_n)$ converges to $f(\sum u_n)$.
- **Raab-Duhamel criterion** is used when **d'Alembert's criterion** gives $k = 1$.
- **Gauss criterion** is used when both **d'Alembert** and **Raab-Duhamel** give inconclusive results.
- **Cauchy's rule** (root test) is more general than **d'Alembert's rule** (ratio test).
- If $\lim_{n \to +\infty} \frac{u_{n+1}}{u_n} = 1$, then $\lim_{n \to +\infty} \sqrt[n]{u_n} = 1$, so Cauchy's rule won't help either.
- The **logarithm criterion** is useful for series involving logarithmic terms.
- A convergent series that is not absolutely convergent is called **semi-convergent**.
- The criteria for **absolute convergence** are the same as those for **series with positive terms**, applied to $\sum_n |u_n|$.
 - Not all series whose general terms contain $(-1)^n$ are alternating series. For example, the series $\sum_{n \geq 0} (-1)^n \cos n$ is not alternating because $\cos n$ does not maintain a constant sign for all $n \geq 0$.
 - There are alternating series in which the term $(-1)^n$ does not appear explicitly. For example, $\sum_{n \geq 1} \frac{\cos n\pi}{\ln n}$ is an alternating series, because for all $n \geq 1$, $\ln n \geq 0$ and for all $n \in \mathbb{N}$, we have $\cos n\pi = \sin(2n+1)\pi = (-1)^n$.