---
aliases:
  - chapter_II
---

## 📚 Course Structure
- Section 1: **Motivation & Area Approximation**
- Section 2: **Riemann Integral Definition**
- Section 3: **Integrable Functions & Properties**

---
## 📐 Equations & Concepts
#### Motivation & Area Approximation
- **Goal:** Compute the area under $y = e^x$ from $x = 0$ to $x = 1$.
- **Rectangle Approximation:**
  - Divide $[0,1]$ into $n$ subintervals of length $1/n$.
  - Lower sum: Use left endpoints $x_{i-1}$, area $\frac{1}{n} e^{\frac{i-1}{n}}$.
  - Upper sum: Use right endpoints $x_i$, area $\frac{1}{n} e^{\frac{i}{n}}$.
  - As $n \to \infty$, both sums approach $e-1$.
- **Conclusion:**
  $$
  \int_0^1 e^x dx = e - 1
  $$

#### Riemann Integral Definition
- **Subdivision:**
  - A subdivision of $[a, b]$ is a sequence $a = x_0 < x_1 < \cdots < x_n = b$.
  - **Regular subdivision:** All intervals have equal length $\frac{b-a}{n}$.
- **Step Function:**
  - $f$ is a step function if there exists a subdivision and constants $c_1, ..., c_n$ such that $f(x) = c_i$ on $[x_{i-1}, x_i]$.
- **Integral of Step Function:**
  $$
  \int_a^b f(x) dx = \sum_{i=1}^n (x_i - x_{i-1}) c_i
  $$
- **Properties:**
  - Linearity: $\int_a^b (af + bg) = a \int_a^b f + b \int_a^b g$
  - Additivity: $\int_a^b f = \int_a^c f + \int_c^b f$
  - Monotonicity: If $f \leq g$, then $\int_a^b f \leq \int_a^b g$

- **Riemann Integral (General Function):**
  - For bounded $f$ on $[a, b]$, define:
    - Lower integral: $I^- = \sup$ of integrals of step functions $\leq f$
    - Upper integral: $I^+ = \inf$ of integrals of step functions $\geq f$
  - $f$ is Riemann integrable if $I^- = I^+$, and this value is $\int_a^b f(x) dx$.

#### Integrable Functions & Properties
- **Integrable Functions:**
  - All step functions are integrable.
  - If $f$ is continuous on $[a, b]$, then $f$ is integrable.
  - If $f$ is monotone on $[a, b]$, then $f$ is integrable.
  - Piecewise continuous or piecewise monotone functions are integrable.
  - Not all bounded functions are integrable (e.g., Dirichlet function).
- **Darboux Sums:**
  - For any subdivision $S$, define lower and upper Darboux sums:
    - $D_S^-(f) = \sum_{i=1}^n (x_i - x_{i-1}) m_i$, $m_i = \inf_{[x_{i-1}, x_i]} f$
    - $D_S^+(f) = \sum_{i=1}^n (x_i - x_{i-1}) M_i$, $M_i = \sup_{[x_{i-1}, x_i]} f$
  - $f$ is integrable iff for every $\varepsilon > 0$, there exists a subdivision $S$ such that $D_S^+(f) - D_S^-(f) < \varepsilon$.
- **Properties of the Integral:**
  - **Chasles Relation:** $\int_a^b f = \int_a^c f + \int_c^b f$
  - **Linearity:** $\int_a^b (af + bg) = a \int_a^b f + b \int_a^b g$
  - **Monotonicity:** If $f \leq g$, then $\int_a^b f \leq \int_a^b g$
  - **Positivity:** If $f \geq 0$, then $\int_a^b f \geq 0$

---
## 📝 Notes
- The Riemann integral is defined as the common limit of lower and upper sums using step functions.
- Continuous, monotone, and piecewise continuous/monotone functions are always integrable.
- The integral measures the signed area between the curve and the $x$-axis.
- The Chasles relation allows splitting the interval of integration.
- Not all bounded functions are integrable (e.g., Dirichlet function is not).
