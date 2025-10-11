---
aliases:
  - chapter_III
---

## 📚 Course Structure
- Section 1: **Couples of Discrete Random Variables**
- Section 2: **Independence of Discrete Random Variables**
- Section 3: **Functions of Two Random Variables**
- Section 4: **Sums of Discrete Random Variables**

---
## 📐 Equations & Concepts
#### Couples of Discrete Random Variables:
- **Joint Law:**
  - The **joint law** of $(X, Y)$ is the set of pairs $((x_i, y_j), p_{i,j})$ where $p_{i,j} = P(X = x_i, Y = y_j)$.
- **Marginal Laws:**
  - Obtained by summing the joint probabilities:
    $$P(X = x_i) = \sum_{j \in J} P(X = x_i, Y = y_j)$$
    $$P(Y = y_j) = \sum_{i \in I} P(X = x_i, Y = y_j)$$
- **Conditional Laws:**
  - The **conditional law of $X$ given $[Y = y]$** is defined by:
    $$P_{[Y=y]}(X = x_i) = \frac{P(X = x_i, Y = y)}{P(Y = y)}$$

#### Independence of Discrete Random Variables:
- **Definition:** $X$ and $Y$ are **independent** if:
  $$\forall (x, y),\quad P(X = x, Y = y) = P(X = x)P(Y = y)$$
- **Property:** If $X$ and $Y$ are independent, then $f(X)$ and $g(Y)$ are independent for any functions $f$, $g$.
- **Mutual Independence:** $X_1, \dots, X_n$ are mutually independent if:
  $$P(X_1 = x_1, \dots, X_n = x_n) = \prod_{k=1}^n P(X_k = x_k)$$

#### Functions of Two Random Variables:
- **Law of $Z = g(X, Y)$:**
  $$P(Z = z_k) = \sum_{(i,j):\, g(x_i,y_j)=z_k} P(X = x_i, Y = y_j)$$
- **Transfer Theorem:**
  $$E(g(X, Y)) = \sum_{(x,y)} g(x, y) P(X = x, Y = y)$$
- **Product Expectation:**
  - $E(XY) = \sum xy P(X = x, Y = y)$
  - If $X$ and $Y$ are independent: $E(XY) = E(X)E(Y)$
- **Covariance:**
  - $\text{cov}(X,Y) = E[(X - E(X))(Y - E(Y))] = E(XY) - E(X)E(Y)$
  - If $X$ and $Y$ are independent, then $\text{cov}(X,Y) = 0$ (but converse is false).
- **Correlation Coefficient:**
  $$\rho(X,Y) = \frac{\text{cov}(X,Y)}{\sigma(X)\sigma(Y)} \in [-1,1]$$

#### Sums of Discrete Random Variables:
- **Linearity of Expectation:**
  $$E(aX + bY) = aE(X) + bE(Y)$$
  $$E(X_1 + \cdots + X_n) = \sum_{i=1}^n E(X_i)$$
- **Variance of a Sum:**
  - $V(X + Y) = V(X) + V(Y) + 2\text{cov}(X,Y)$
  - If $X$ and $Y$ are independent: $V(X + Y) = V(X) + V(Y)$
  - For $n$ independent variables: $V(X_1 + \cdots + X_n) = \sum_{i=1}^n V(X_i)$
- **Sums of Independent Variables:**
  - If $X \sim B(n,p)$, $Y \sim B(m,p)$ are independent, then $X + Y \sim B(n+m, p)$.
  - If $X \sim P(\lambda)$, $Y \sim P(\mu)$ are independent, then $X + Y \sim P(\lambda + \mu)$.

---
## 📝 Notes
- The joint law fully determines the marginal and conditional laws.
- Independence implies zero covariance, but zero covariance does not imply independence.
- The correlation coefficient $\rho$ measures the strength of linear dependence.
- Expectation is always linear, but variance is only additive when variables are uncorrelated (especially when independent).
- Sums of independent Binomials (with same $p$) or Poissons are again Binomial or Poisson.