## 📚 Course Structure
- Section 1: **Key Skills & Knowledge**
- Section 2: **Continuous Distributions Reference**

---
## 📐 Equations & Concepts
#### Key Skills & Knowledge:
- **Verifying Probability Density Functions:**
  - Check: $f(x) \geq 0$, continuity (except finite points), $\int_{-\infty}^{+\infty} f(t) dt = 1$
- **From Density to CDF:**
  - $F(x) = \int_{-\infty}^{x} f(t) dt$
- **From CDF to Density:**
  - If $F$ is continuous and $C^1$ except at finite points, then $X$ has density $f(x) = F'(x)$
- **Probability Calculations:**
  - $P(X = a) = 0$ for any $a \in \mathbb{R}$
  - $P(X \leq a) = P(X < a) = F(a) = \int_{-\infty}^{a} f(t) dt$
  - $P(X \geq a) = P(X > a) = 1 - F(a) = \int_{a}^{+\infty} f(t) dt$
  - $P(a \leq X \leq b) = F(b) - F(a) = \int_{a}^{b} f(t) dt$
- **Standardized Variable:**
  - $X^* = \frac{X - E(X)}{\sigma(X)}$

#### Continuous Distributions Reference:
- **Uniform $U([a, b])$:**
  - Density: $f(t) = \frac{1}{b-a}$ for $t \in [a,b]$, 0 otherwise
  - CDF: $F(x) = \frac{x-a}{b-a}$ for $x \in [a,b]$
  - $E(X) = \frac{a+b}{2}$, $V(X) = \frac{(b-a)^2}{12}$
- **Exponential $\mathcal{E}(\lambda)$:**
  - Density: $f(t) = \lambda e^{-\lambda t}$ for $t \geq 0$, 0 otherwise
  - CDF: $F(x) = 1 - e^{-\lambda x}$ for $x \geq 0$
  - $E(X) = \frac{1}{\lambda}$, $V(X) = \frac{1}{\lambda^2}$
- **Standard Normal $\mathcal{N}(0,1)$:**
  - Density: $f(t) = \frac{1}{\sqrt{2\pi}} e^{-t^2/2}$
  - CDF: $\Phi(x)$
  - $E(X) = 0$, $V(X) = 1$
  - Property: $\Phi(x) + \Phi(-x) = 1$
- **Normal $\mathcal{N}(m, \sigma^2)$:**
  - Density: $f(t) = \frac{1}{\sigma\sqrt{2\pi}} \exp\left(-\frac{(t-m)^2}{2\sigma^2}\right)$
  - $E(X) = m$, $V(X) = \sigma^2$
  - Standardization: If $X \sim \mathcal{N}(m,\sigma^2)$, then $X^* \sim \mathcal{N}(0,1)$

---
## 📝 Notes
- Always verify the 3 conditions when proving a function is a probability density
- For continuous variables, probability at a point is always zero
- The CDF completely characterizes a continuous random variable
- Know how to transform variables: $Y = g(X)$ and find its distribution
- Standard normal CDF $\Phi(x)$ must be used with statistical tables
- All normal distributions can be standardized to $\mathcal{N}(0,1)$
- Memorize the key properties and formulas for uniform, exponential, and normal distributions