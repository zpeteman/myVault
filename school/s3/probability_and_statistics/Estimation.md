---
aliases:
  - chapter_VI
---

## 📚 Course Structure
- Section 1: **Point Estimation**
- Section 2: **Confidence Intervals**

---
## 📐 Equations & Concepts
#### Point Estimation:
- **n-Sample:**
  - $(X_1, \dots, X_n)$ are i.i.d. with same distribution as $X$ (parent distribution)
- **Estimator & Estimate:**
  - **Estimator:** Random variable $T_n = f(X_1, \dots, X_n)$
  - **Estimate:** Realized value $f(x_1, \dots, x_n)$ from data
  - **Sample Mean:** $\bar{X}_n = \frac{1}{n}\sum_{i=1}^n X_i$
- **Estimator Quality:**
  - **Bias:** $b(T_n) = E(T_n) - \theta$
    - Unbiased if $b(T_n) = 0$ ($E(T_n) = \theta$)
  - **Quadratic Risk:** $r(T_n) = E[(T_n - \theta)^2]$
    - $r(T_n) = V(T_n) + [b(T_n)]^2$
    - For unbiased estimators: $r(T_n) = V(T_n)$
- **Mean Estimation:**
  - Sample mean $\bar{X}_n$ is unbiased for population mean $m$
  - $r(\bar{X}_n) = \frac{V(X)}{n} \to 0$ as $n \to \infty$

#### Confidence Intervals:
- **Definition:**
  - $[U_n, V_n]$ is a confidence interval for $\theta$ at level $1-\alpha$ if:
    $$P(U_n \leq \theta \leq V_n) \geq 1 - \alpha$$
- **Using Bienaymé-Tchebychev:**
  - For unbiased estimator $T_n$:
    $$P(T_n - \varepsilon \leq \theta \leq T_n + \varepsilon) \geq 1 - \frac{V(T_n)}{\varepsilon^2}$$
  - If $V(T_n) \leq v_n$, then:
    $$P(T_n - \varepsilon \leq \theta \leq T_n + \varepsilon) \geq 1 - \frac{v_n}{\varepsilon^2}$$
  - For Bernoulli: $V(\bar{X}_n) = \frac{\theta(1-\theta)}{n} \leq \frac{1}{4n}$
- **Using Normal Approximation:**
  - For $n \geq 30$, $\bar{X}_n^* = \frac{\bar{X}_n - m}{\sigma/\sqrt{n}} \approx \mathcal{N}(0,1)$
  - Find $t_\alpha$ such that $\Phi(t_\alpha) = 1 - \frac{\alpha}{2}$
    - For $\alpha = 0.05$: $t_\alpha \approx 1.96$
  - Confidence interval:
    $$\left[ \bar{X}_n - \frac{\sigma t_\alpha}{\sqrt{n}}, \bar{X}_n + \frac{\sigma t_\alpha}{\sqrt{n}} \right]$$

---
## 📝 Notes
- An estimator is a random variable; an estimate is its realized value
- Unbiasedness means correct on average, but individual estimates can be far from true value
- Quadratic risk combines variance and bias squared
- Sample mean becomes better estimator as sample size increases
- Confidence intervals give range where parameter likely lies, not probability about parameter
- Normal approximation gives tighter intervals than Bienaymé-Tchebychev
- For Bernoulli, maximum variance occurs at $p = 0.5$ ($\sigma^2 \leq 0.25$)
- Common confidence level: 95% ($\alpha = 0.05$, $t_\alpha \approx 1.96$)