---
aliases:
  - chapter_V
---

## 📚 Course Structure
- Section 1: **Inequalities & Convergence Theorems**
- Section 2: **Approximations of Probability Distributions**

---
## 📐 Equations & Concepts
#### Inequalities & Convergence Theorems:
- **Bienaymé-Tchebychev Inequality:**
  - If $X$ has finite variance, then:
    $$\forall \varepsilon > 0, \quad P(|X - E(X)| \geq \varepsilon) \leq \frac{V(X)}{\varepsilon^2}$$
- **Weak Law of Large Numbers:**
  - Let $(X_n)$ be i.i.d. with mean $m$ and variance $\sigma^2$. Define $\bar{X}_n = \frac{1}{n}\sum_{i=1}^n X_i$. Then:
    $$\forall \varepsilon > 0, \quad \lim_{n \to \infty} P(|\bar{X}_n - m| \geq \varepsilon) = 0$$
- **Convergence in Law:**
  - $(X_n)$ converges in law to $X$ if $F_{X_n}(x) \to F_X(x)$ at all continuity points of $F_X$
  - For discrete variables: $\lim_{n \to \infty} P(X_n = k) = P(X = k)$ for all $k$
- **Central Limit Theorem:**
  - Let $(X_n)$ be i.i.d. with mean $m$ and variance $\sigma^2$. Define:
    $$S_n = \sum_{k=1}^n X_k, \quad S_n^* = \frac{S_n - nm}{\sigma\sqrt{n}}$$
    Then $S_n^*$ converges in law to $\mathcal{N}(0,1)$
  - Practical rule: For $n \geq 30$, $S_n^* \approx \mathcal{N}(0,1)$

#### Approximations of Probability Distributions:
- **Hypergeometric → Binomial:**
  - $H(N, n, p) \approx B(n, p)$ when $N \geq 10n$
  - Justified by convergence in law
- **Binomial → Poisson:**
  - $B(n, p) \approx \mathcal{P}(\lambda)$ where $\lambda = np$
  - Valid when $n \geq 30$ and $p \leq 0.1$
  - "Law of rare events"
- **Binomial → Normal:**
  - $B(n, p) \approx \mathcal{N}(np, npq)$
  - Valid when $n \geq 30$, $np \geq 5$, $nq \geq 5$
  - Use standardization: $X^* = \frac{X - np}{\sqrt{npq}} \approx \mathcal{N}(0,1)$
  - **Continuity correction:** $P(X = k) \approx P(k - 0.5 < N < k + 0.5)$
- **Poisson → Normal:**
  - $\mathcal{P}(\lambda) \approx \mathcal{N}(\lambda, \lambda)$ when $\lambda \geq 18$
  - Standardize: $\frac{X - \lambda}{\sqrt{\lambda}} \approx \mathcal{N}(0,1)$

---
## 📝 Notes
- Bienaymé-Tchebychev gives a bound, not an exact probability
- Law of Large Numbers justifies frequency interpretation of probability
- Central Limit Theorem explains why normal distribution appears everywhere
- Continuity correction improves accuracy when approximating discrete by continuous distributions
- Approximation conditions are practical rules, not strict mathematical boundaries
- Poisson approximation works best for rare events ($p$ small)
- Normal approximation works best when distribution is not too skewed ($np$ and $nq$ both ≥ 5)