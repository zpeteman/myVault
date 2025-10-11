---
aliases:
  - chapter_IV
---

## 📚 Course Structure
- Section 1: **Continuous Random Variables & Density**
- Section 2: **Moments of Continuous Random Variables**
- Section 3: **Common Continuous Distributions**
- Section 4: **Functions of Continuous Random Variables**

---
## 📐 Equations & Concepts
#### Continuous Random Variables & Density:
- **Definition:** A random variable $X$ is **continuous** if there exists a **density function** $f_X$ such that:
  1. $f_X(x) \geq 0$
  2. $f_X$ is continuous except possibly at finitely many points
  3. $\int_{-\infty}^{+\infty} f_X(t)  dt = 1$
  4. $F_X(x) = P(X \leq x) = \int_{-\infty}^{x} f_X(t)  dt$
- **Key Properties:**
  - $P(X = a) = 0$ for any $a \in \mathbb{R}$
  - $P(a \leq X \leq b) = \int_a^b f_X(t)  dt$
  - $F_X$ is continuous and non-decreasing
- **Independence:** $X_1, \dots, X_n$ are independent if for all reals $(x_1, \dots, x_n)$:
  $$P(X_1 \leq x_1, \dots, X_n \leq x_n) = \prod_{k=1}^n P(X_k \leq x_k)$$

#### Moments of Continuous Random Variables:
- **Expectation:**
  $$E(X) = \int_{-\infty}^{+\infty} t f(t)  dt \quad \text{(if absolutely convergent)}$$
  - **Linearity:** $E(aX + b) = aE(X) + b$
  - $E(X + Y) = E(X) + E(Y)$
- **Moment of order $r$:**
  $$m_r(X) = \int_{-\infty}^{+\infty} x^r f(x)  dx \quad \text{(if absolutely convergent)}$$
- **Variance:**
  $$V(X) = E[(X - E(X))^2] = E(X^2) - [E(X)]^2$$
  - $V(aX + b) = a^2 V(X)$
- **Standardized Variable:**
  $$X^* = \frac{X - E(X)}{\sigma(X)}$$

#### Common Continuous Distributions:
- **Uniform Distribution $U([a, b])$:**
  - Density: $f(x) = \frac{1}{b-a}$ for $x \in [a,b]$, 0 otherwise
  - CDF: $F(x) = \frac{x-a}{b-a}$ for $x \in [a,b]$
  - Moments: $E(X) = \frac{a+b}{2}$, $V(X) = \frac{(b-a)^2}{12}$
- **Exponential Distribution $\mathcal{E}(\lambda)$:**
  - Density: $f(x) = \lambda e^{-\lambda x}$ for $x \geq 0$, 0 otherwise
  - CDF: $F(x) = 1 - e^{-\lambda x}$ for $x \geq 0$
  - Memoryless property: $P(X > s+t | X > s) = P(X > t)$
  - Moments: $E(X) = \frac{1}{\lambda}$, $V(X) = \frac{1}{\lambda^2}$
- **Normal Distribution $\mathcal{N}(m, \sigma^2)$:**
  - Density: $f(x) = \frac{1}{\sigma\sqrt{2\pi}} \exp\left(-\frac{(x-m)^2}{2\sigma^2}\right)$
  - Standard Normal: $\mathcal{N}(0,1)$ with density $\phi(x) = \frac{1}{\sqrt{2\pi}} e^{-x^2/2}$
  - CDF symmetry: $\Phi(-x) = 1 - \Phi(x)$
  - Moments: $E(X) = m$, $V(X) = \sigma^2$
  - Standardization: If $X \sim \mathcal{N}(m,\sigma^2)$, then $\frac{X-m}{\sigma} \sim \mathcal{N}(0,1)$

#### Functions of Continuous Random Variables:
- **Transfer Theorem:**
  $$E(g(X)) = \int_{-\infty}^{+\infty} g(t)f(t)  dt \quad \text{(if absolutely convergent)}$$
- **Affine Transformation ($Y = aX + b$):**
  - Density: $g(y) = \frac{1}{|a|} f\left(\frac{y-b}{a}\right)$
- **Square Transformation ($Y = X^2$):**
  - Density: $g(y) = \frac{1}{2\sqrt{y}}[f(\sqrt{y}) + f(-\sqrt{y})]$ for $y > 0$, 0 otherwise
- **Exponential Transformation ($Y = e^X$):**
  - Density: $g(y) = \frac{1}{y} f(\ln y)$ for $y > 0$, 0 otherwise

---
## 📝 Notes
- A density function is not unique; functions differing at finitely many points are equivalent.
- For continuous variables, $P(X = a) = 0$ for any specific value $a$.
- The normal distribution CDF cannot be expressed in terms of elementary functions.
- The exponential distribution is "memoryless" - the future is independent of the past.
- All normal distributions are related to the standard normal via standardization.
- When transforming variables, always find the new CDF first, then differentiate to get the density.