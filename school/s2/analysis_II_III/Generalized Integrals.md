---
aliases:
  - chapter_IV
---

## 📚 Course Structure
- Section 1: **Generalized Integrals: Motivation & Definitions**
- Section 2: **Properties of Generalized Integrals**
- Section 3: **Convergence Criteria & Comparison Theorems**

---
## 📐 Equations & Concepts
#### Generalized Integrals: Motivation & Definitions
- **Motivation:**
  - Standard integrals require functions to be bounded on closed, bounded intervals $[a, b]$.
  - Some functions (e.g., $f(x) = \frac{1}{x}$ on $(0,1]$) are not bounded, or are defined on unbounded intervals.
  - **Goal:** Extend the definition of the integral to such cases.

- **Locally Integrable:**
  - $f$ is locally integrable on $I$ if $f$ is integrable on every closed, bounded subinterval of $I$.
  - Examples: $f(x) = \frac{1}{x}$ on $(0,1]$; $g(x) = \frac{1}{x^2+1}$ on $\mathbb{R}$; $h(x) = x e^{-x^2}$ on $\mathbb{R}$.
  - Counterexample: Dirichlet function $Q(x)$ is not locally integrable.

- **Generalized Integral (Improper Integral):**
  - For $f$ locally integrable on $(a, b)$:
    - $\int_a^b f(t) dt$ is **convergent** if $\lim_{x \to b^-} \int_a^x f(t) dt$ exists and is finite.
    - If not, the integral is **divergent**.
  - For $f$ on $(a, b]$, $\int_a^b f(t) dt = \lim_{x \to a^+} \int_x^b f(t) dt$ if the limit exists.
  - For $f$ on $(-\infty, b]$, $\int_{-\infty}^b f(t) dt = \lim_{a \to -\infty} \int_a^b f(t) dt$.
  - For $f$ on $[a, \infty)$, $\int_a^{\infty} f(t) dt = \lim_{b \to \infty} \int_a^b f(t) dt$.

- **Examples:**
  - $\int_0^1 \frac{1}{1+t^2} dt = \arctan(1) - \arctan(0) = \frac{\pi}{4}$ (converges)
  - $\int_0^1 \frac{1}{t} dt$ diverges (limit goes to $+\infty$)
  - $\int_0^1 \ln t dt = [t \ln t - t]_0^1 = -1$ (converges)

#### Properties of Generalized Integrals
- **Linearity:**
  - If $\int_a^b f(t) dt$ and $\int_a^b g(t) dt$ converge, then $\int_a^b (\alpha f + \beta g)(t) dt$ converges and equals $\alpha \int_a^b f(t) dt + \beta \int_a^b g(t) dt$.
- **Chasles Relation:**
  - If $c \in (a, b)$, $\int_a^b f(t) dt = \int_a^c f(t) dt + \int_c^b f(t) dt$ (if all terms converge).
- **Monotonicity:**
  - If $f \leq g$ on $(a, b)$ and both integrals converge, then $\int_a^b f \leq \int_a^b g$.
- **Positivity:**
  - If $f \geq 0$ and $\int_a^b f$ converges, then $\int_a^b f \geq 0$.
- **Integration by Parts:**
  - If $u, v$ are $C^1$ and $\lim_{x \to b^-} u(x)v(x)$ exists, then
    $$
    \int_a^b u(t)v'(t) dt = [u(t)v(t)]_a^b - \int_a^b u'(t)v(t) dt
    $$
- **Change of Variable:**
  - If $x = \varphi(t)$ is $C^1$ and bijective, then
    $$
    \int_a^b f(x) dx = \int_{\varphi^{-1}(a)}^{\varphi^{-1}(b)} f(\varphi(t)) \varphi'(t) dt
    $$

#### Convergence Criteria & Comparison Theorems
- **Primitive Criterion:**
  - $\int_a^b f(t) dt$ converges iff $\lim_{x \to b^-} F(x)$ exists and is finite, where $F$ is a primitive of $f$.
- **Comparison Theorem:**
  - If $0 \leq f(t) \leq g(t)$ and $\int_a^b g(t) dt$ converges, then $\int_a^b f(t) dt$ converges.
  - If $\int_a^b f(t) dt$ diverges, so does $\int_a^b g(t) dt$.
- **Riemann and Bertrand Integrals:**
  - $\int_1^{\infty} \frac{1}{t^\alpha} dt$ converges iff $\alpha > 1$.
  - $\int_0^1 \frac{1}{t^\alpha} dt$ converges iff $\alpha < 1$.
  - $\int_1^{\infty} \frac{1}{t (\ln t)^\beta} dt$ converges iff $\beta > 1$.
- **Absolute Convergence:**
  - If $\int_a^b |f(t)| dt$ converges, then $\int_a^b f(t) dt$ converges (but not always the converse).
- **Abel's Rule:**
  - If $f$ is positive, decreasing, $\lim_{x \to b^-} f(x) = 0$, and $\int_a^b g(t) dt$ is bounded, then $\int_a^b f(t)g(t) dt$ converges.

---
## 📝 Notes
- Generalized (improper) integrals extend the Riemann integral to unbounded intervals or unbounded functions.
- Convergence depends on the behavior near singularities or at infinity.
- Use comparison with known integrals (Riemann, Bertrand) to test convergence.
- Integration by parts and substitution remain valid for generalized integrals, with care for limits.
- Absolute convergence implies convergence, but not vice versa (semi-convergent integrals exist).
- Always check the nature of the singularity and use the appropriate convergence test.
