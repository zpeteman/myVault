---
aliases:
  - chapter_I
---

## 📚 Course Structure
- Section 1: **Taylor Formulas & Applications**
- Section 2: **Successive Derivatives & Taylor-Lagrange**
- Section 3: **Limited Developments (DL) & Operations**

---
## 📐 Equations & Concepts
#### Taylor Formulas & Applications
- **Rolle's Theorem:** If $f$ is continuous on $[a, b]$, differentiable on $(a, b)$, and $f(a) = f(b)$, then there exists $c \in (a, b)$ such that $f'(c) = 0$.
- **Mean Value Theorem (MVT):** If $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists $c \in (a, b)$ such that $f(b) - f(a) = (b - a)f'(c)$.
- **Monotonicity:**
  - $f$ increasing on $I$ if $f'(x) \geq 0$ for all $x \in I$.
  - $f$ decreasing on $I$ if $f'(x) \leq 0$ for all $x \in I$.
- **L'Hospital's Rule:** If $\lim_{x \to a} f(x) = \lim_{x \to a} g(x) = 0$ and $g'(x) \neq 0$ near $a$, then $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$.

#### Successive Derivatives & Taylor-Lagrange
- **Successive Derivatives:**
  - $f$ is $n$ times differentiable if $f^{(n)}$ exists.
  - $f^{(0)} = f$, $f^{(1)} = f'$, $f^{(2)} = f''$, etc.
- **Leibniz Formula:**
  - $(fg)^{(n)} = \sum_{k=0}^n \binom{n}{k} f^{(n-k)} g^{(k)}$
- **Class $C^n$ Functions:**
  - $f$ is $C^n$ if $f^{(n)}$ is continuous.
- **Taylor-Lagrange Formula:**
  - If $f$ is $n+1$ times differentiable on $[a, b]$, then:
    $$
    f(b) = f(a) + (b-a)f'(a) + \frac{(b-a)^2}{2!}f''(a) + \cdots + \frac{(b-a)^n}{n!}f^{(n)}(a) + \frac{(b-a)^{n+1}}{(n+1)!}f^{(n+1)}(c)
    $$
    for some $c \in (a, b)$.
- **Maclaurin Formula:**
  - Special case of Taylor at $a=0$:
    $$
    f(x) = f(0) + x f'(0) + \frac{x^2}{2!}f''(0) + \cdots + \frac{x^n}{n!}f^{(n)}(0) + \frac{x^{n+1}}{(n+1)!}f^{(n+1)}(\xi)
    $$
    for some $\xi \in (0, x)$.

#### Limited Developments (DL) & Operations
- **DL at 0 (Order $n$):**
  - $f(x) = a_0 + a_1 x + \cdots + a_n x^n + o(x^n)$
  - $a_k = \frac{f^{(k)}(0)}{k!}$
- **DL at $x_0$ (Order $n$):**
  - $f(x) = a_0 + a_1(x-x_0) + \cdots + a_n(x-x_0)^n + o((x-x_0)^n)$
- **DL at $\infty$:**
  - $f(x) = a_0 + a_1 x + \cdots + a_n x^n + o(x^n)$ as $x \to \infty$
- **DL Operations:**
  - **Sum:** Add polynomials, keep $o(x^n)$
  - **Product:** Multiply polynomials, keep terms up to $x^n$
  - **Quotient:** Divide polynomials, keep terms up to $x^n$
  - **Composition:** Substitute one DL into another, keep terms up to $x^n$
  - **Derivative:** Differentiate the polynomial part, remainder becomes $o(x^{n-1})$
  - **Primitive:** Integrate the polynomial part, remainder becomes $o(x^{n+1})$
- **DL Examples (Order $n$):**
  - $e^x = 1 + x + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + o(x^n)$
  - $\sin x = x - \frac{x^3}{3!} + \cdots + o(x^n)$
  - $\cos x = 1 - \frac{x^2}{2!} + \cdots + o(x^n)$
  - $\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} + o(x^n)$

---
## 📝 Notes
- Taylor and Maclaurin formulas approximate functions by polynomials near a point.
- The remainder term estimates the error of approximation.
- DLs (limited developments) are used for approximations, limits, and studying function behavior.
- Operations on DLs follow polynomial algebra, keeping only terms up to the desired order.
- Convexity: $f$ is convex if $f''(x) \geq 0$; concave if $f''(x) \leq 0$.
- Extremum conditions: If $f'(a) = 0$ and $f''(a) > 0$, $a$ is a local minimum; if $f''(a) < 0$, $a$ is a local maximum.
