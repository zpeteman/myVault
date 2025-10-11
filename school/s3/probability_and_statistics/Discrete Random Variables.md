---
aliases:
  - chapter_II
---

## 📚 Course Structure
- Section 1: **General Concepts on Discrete Random Variables**
- Section 2: **Usual Discrete Distributions**

---
## 📐 Equations & Concepts
#### General Concepts on Discrete Random Variables:
- **Definition & Properties:**
	- **Real Discrete Random Variable:** Let $(\Omega, \mathcal{A})$ be a probability space. A **real discrete random variable** is a mapping $X$ from $\Omega$ to $\mathbb{R}$ such that:
	  1. $X(\Omega) = \\{x_i / i \in I\\}$ where $I = \mathbb{N}$, $\mathbb{Z}$, or a finite subset.
	  2. For all $x \in X(\Omega)$, $\\{\omega \in \Omega / X(\omega) = x\\} \in \mathcal{A}$.
	- **Vocabulary:** $X(\Omega)$ is the set of values taken by $X$. If $I$ is finite, $X$ is a finite discrete random variable; otherwise, it's infinite.
	- **Property:** For any interval $J$ of $\mathbb{R}$, the set $\\{\omega \in \Omega / X(\omega) \in J\\}$ is an event, noted $[X \in J]$.
- **Probability Distribution:**
	- **Definition:** The **probability distribution** (or law) of a discrete random variable $X$ is the set of pairs $(x_i, p_i)$ where $x_i \in X(\Omega)$ and $p_i = P(X = x_i)$.
	- **Key Property:** The family of events $([X = x_i])_{i \in I}$ is a complete system of events. Therefore: $$\sum_{i \in I} P(X = x_i) = 1$$
- **Cumulative Distribution Function:**
	- **Definition:** The **cumulative distribution function** of $X$ is the application $F: \mathbb{R} \to \mathbb{R}$ defined by $F(x) = P(X \leq x)$.
	- **Properties:**
	  1. $\forall x \in \mathbb{R}, F(x) \in [0; 1]$
	  2. $F$ is non-decreasing.
	  3. $\lim_{x \to -\infty} F(x) = 0$ and $\lim_{x \to +\infty} F(x) = 1$.
	  4. $\forall (a, b) \in \mathbb{R}^2, P(a < X \leq b) = F(b) - F(a)$.
	- **Characterization of the Law:** If the $x_i$ are in increasing order, then for all $i$: $$P(X = x_i) = F(x_i) - F(x_{i-1})$$
- **Function of a Random Variable:**
	- **Definition:** Let $X$ be a discrete random variable and $g$ a function defined on $X(\Omega)$. The variable $Y = g(X)$ is defined by $Y(\omega) = g(X(\omega))$.
	- **Property:** $Y$ is a discrete random variable with $Y(\Omega) = \\{ g(x_i)/i \in I \\}$ and for all $y \in Y(\Omega)$: $$P(Y = y) = \sum_{i/g(x_i) = y} P(X = x_i)$$
- **Moments of a Discrete Random Variable:**
	- **Expectation:**
		- **Definition:** $X$ has an **expectation** if $I$ is finite or if the series $\sum x_i P(X = x_i)$ is absolutely convergent. Then: $$E(X) = \sum_{i \in I} x_i P(X = x_i)$$
		- **Transfer Theorem:** If $X$ has an expectation, then for any function $g$, $g(X)$ has an expectation given by: $$E(g(X)) = \sum_{i \in I} g(x_i)P(X = x_i)$$
		- **Linearity:** For any $(a, b) \in \mathbb{R}^2$, $E(aX + b) = aE(X) + b$.
		- **Centered Variable:** A variable with $E(X) = 0$ is called **centered**. The variable $X - E(X)$ is the centered variable associated with $X$.
	- **Moment of order $r$:**
		- **Definition:** If $X^r$ has an expectation, then $X$ has a **moment of order $r$**, noted $m_r(X) = E(X^r)$.
		- **Property:** If $X$ has a moment of order $r$, then it has moments of order $s$ for all $s \in [1; r]$.
	- **Variance & Standard Deviation:**
		- **Definition:** If $X$ has an expectation and $(X - E(X))^2$ has an expectation, then the **variance** is: $$V(X) = E\left((X - E(X))^2\right)$$ The **standard deviation** is $\sigma(X) = \sqrt{V(X)}$.
		- **Koenig's Formula (Huygens):** $$V(X) = E(X^2) - E(X)^2$$
		- **Property:** For any $(a, b) \in \mathbb{R}^2$, $V(aX + b) = a^2 V(X)$.
		- **Standardized Variable:** A variable with $E(X) = 0$ and $\sigma(X) = 1$ is called **centered and reduced**. If $X$ has a non-zero variance, the variable $X^* = \frac{X - E(X)}{\sigma(X)}$ is the centered and reduced variable associated with $X$.

#### Usual Discrete Distributions:
- **Finite Discrete Distributions:**
	- **Bernoulli Distribution:**
		- **Context:** Models a single trial with success probability $p$.
		- **Definition:** $X \sim B(1, p)$ if $P(X=1)=p$ and $P(X=0)=1-p$.
		- **Moments:** $E(X) = p$, $V(X) = p(1-p)$.
	- **Binomial Distribution:**
		- **Context:** Counts the number of successes in $n$ independent trials, each with success probability $p$.
		- **Definition:** $X \sim B(n, p)$ if for $k = 0, 1, ..., n$: $$P(X = k) = \binom{n}{k} p^k(1 - p)^{n-k}$$
		- **Moments:** $E(X) = np$, $V(X) = np(1-p)$.
		- **Theorem:** The sum of $n$ independent Bernoulli($p$) variables follows $B(n, p)$.
	- **Hypergeometric Distribution:**
		- **Context:** Counts the number of successes in $n$ draws without replacement from a population of size $N$ containing $M$ successes. ($p = M/N$).
		- **Definition:** $X \sim H(N, n, p)$ if for applicable $k$: $$P(X = k) = \frac{\binom{Np}{k} \binom{N - Np}{n - k}}{\binom{N}{n}}$$
		- **Moments:** $E(X) = np$.
	- **Uniform Distribution:**
		- **Context:** Models an equiprobable outcome from a finite set.
		- **Definition:** $X$ is uniform on $[1;n]$ if $P(X = k) = \frac{1}{n}$ for $k = 1, 2, ..., n$.
		- **Moments:** $E(X) = \frac{n + 1}{2}$, $V(X) = \frac{n^2 - 1}{12}$.
- **Infinite Discrete Distributions:**
	- **Geometric Distribution:**
		- **Context:** Counts the number of trials needed to get the first success in independent trials with success probability $p$.
		- **Definition:** $X \sim G(p)$ if for $n \in \mathbb{N}^*$: $$P(X = n) = (1 - p)^{n-1}p$$
		- **Moments:** $E(X) = \frac{1}{p}$, $V(X) = \frac{1 - p}{p^2}$.
	- **Poisson Distribution:**
		- **Context:** Often models the number of rare events occurring in a fixed interval.
		- **Definition:** $X \sim P(\lambda)$ if for $n \in \mathbb{N}$: $$P(X = n) = \frac{e^{-\lambda}\lambda^n}{n!}$$
		- **Moments:** $E(X) = \lambda$, $V(X) = \lambda$.

---
## 📝 Notes
- The probability of never getting a 6 when rolling a die repeatedly is 0, which allows us to define the geometric random variable on $\mathbb{N}^*$ instead of $\mathbb{N}^* \cup \{+\infty\}$.
- The cumulative distribution function $F(x)$ for a discrete variable is a non-decreasing step function.
- Koenig's formula is the most practical way to calculate variance.
- A variable can have an expectation but not a variance (see Example 10).
- The sum of probabilities for all possible values of a discrete random variable must always equal 1. This is a crucial check for the consistency of a calculated distribution.
- The standardized variable $X^*$ is very useful for convergence theorems and statistical estimation.