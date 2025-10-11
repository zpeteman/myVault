---
aliases:
  - chapter_III
---

## 📚 Course Structure
- Section 1: **Primitives of a Function**
- Section 2: **Fundamental Theorem of Calculus**
- Section 3: **Integration Techniques (By Parts & Substitution)**
- Section 4: **Primitives of Rational Fractions**
- Section 5: **Primitives Involving Trigonometric Functions**

---
## 📐 Equations & Concepts
#### Primitives of a Function
- **Primitive (Antiderivative):** $F$ is a primitive of $f$ on $I$ if $F'(x) = f(x)$ for all $x \in I$.
- **Finding Primitives:** The operation is the inverse of differentiation.
- **Examples:**
  - $f(x) = x^2 \implies F(x) = \frac{x^3}{3} + c$
  - $f(x) = x \implies F(x) = \frac{x^2}{2} + c$
  - $f(x) = e^x \implies F(x) = e^x + c$
- **All Primitives:** If $F$ is a primitive, all primitives are $F + c$ with $c \in \mathbb{R}$.
- **Notation:** $\int f(x) dx$ denotes a primitive of $f$; $\int_a^b f(x) dx = F(b) - F(a)$ if $F$ is a primitive of $f$.

#### Fundamental Theorem of Calculus
- If $f$ is continuous on $[a, b]$, then $F(x) = \int_a^x f(t) dt$ is a primitive of $f$ on $[a, b]$ and $\int_a^b f(x) dx = F(b) - F(a)$.
- **Examples:**
  - $\int_0^1 e^x dx = e - 1$
  - $\int_0^1 x^2 dx = \frac{1}{3}$
- **Uniqueness:** $F(x) = \int_a^x f(t) dt$ is the unique primitive vanishing at $x = a$.

#### Integration Techniques (By Parts & Substitution)
- **Integration by Parts:**
  - $\int_a^b u(x)v'(x) dx = [u(x)v(x)]_a^b - \int_a^b u'(x)v(x) dx$
  - For primitives: $\int u(x)v'(x) dx = u(x)v(x) - \int u'(x)v(x) dx$
- **Substitution (Change of Variable):**
  - If $x = \varphi(t)$, $dx = \varphi'(t) dt$, then $\int f(x) dx = \int f(\varphi(t)) \varphi'(t) dt$
  - For definite integrals: $\int_a^b f(x) dx = \int_{\varphi^{-1}(a)}^{\varphi^{-1}(b)} f(\varphi(t)) \varphi'(t) dt$
- **Even/Odd and Periodic Functions:**
  - If $f$ is even: $\int_{-a}^a f(x) dx = 2 \int_0^a f(x) dx$
  - If $f$ is odd: $\int_{-a}^a f(x) dx = 0$
  - For $T$-periodic $f$: $\int_a^{a+T} f(x) dx = \int_0^T f(x) dx$

#### Primitives of Rational Fractions
- **Decomposition:** Any rational function $\frac{P(x)}{Q(x)}$ can be written as a sum of polynomials and simple fractions.
- **Integration Cases:**
  - Denominator with real distinct roots: $\int \frac{1}{x-a} dx = \ln|x-a| + c$
  - Double root: $\int \frac{1}{(x-a)^2} dx = -\frac{1}{x-a} + c$
  - No real roots: $\int \frac{1}{x^2 + a^2} dx = \frac{1}{a} \arctan\left(\frac{x}{a}\right) + c$
- **Example:** $\int \frac{2x+1}{x^2+x+1} dx = \ln(x^2+x+1) + \frac{2}{\sqrt{3}} \arctan\left(\frac{2x+1}{\sqrt{3}}\right) + c$

#### Primitives Involving Trigonometric Functions
- **Polynomials in $\sin x$ and $\cos x$:**
  - Use substitution if one exponent is odd; linearize if both are even.
  - Example: $\int \sin x \cos^2 x dx$ (substitute $t = \cos x$)
  - Example: $\int \cos^2 x \sin^4 x dx$ (linearize powers)

---
## 📝 Notes
- Every continuous function on an interval has at least one primitive.
- The set of all primitives differs by a constant.
- Integration by parts and substitution are key tools for computing integrals.
- Rational functions can always be integrated using partial fraction decomposition.
- For trigonometric integrals, use substitution or linearization depending on the powers.
- Not all integrable functions have primitives expressible in terms of elementary functions (e.g., $\int e^{x^2} dx$).
