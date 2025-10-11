---
aliases:
  - chapter_V
---

## 📚 Course Structure
- Section 1: **General Differential Equations**
- Section 2: **First Order Equations (Separable & Linear)**
- Section 3: **Second Order Linear Equations (Constant Coefficients)**
- Section 4: **Physical Applications (Free Fall, Parachutist, Oscillator)**

---
## 📐 Equations & Concepts
#### General Differential Equations
- **Definition:** A differential equation relates an unknown function $y$ of $x$ (or $t$) to its derivatives $y', y'', ...$ and possibly $x$ or $t$.
- **Types:**
  - **ODE (Ordinary):** $y$ depends on one variable.
  - **PDE (Partial):** $y$ depends on several variables.
- **Order $n$:** $F(x, y, y', ..., y^{(n)}) = 0$.
- **Solution:** A function $y(x)$, $n$ times differentiable, that satisfies the equation.

#### First Order Equations (Separable & Linear)
- **Separable Equations:** Can be written as $g(y) y' = f(x)$ or $y' = f(x)g(y)$.
  - **Method:** Separate variables, integrate both sides: $\int g(y) dy = \int f(x) dx + c$.
  - **Example:** $y' = x^2 y$ becomes $\frac{dy}{y} = x^2 dx$.
- **Linear First Order:** $y' + a(x)y = b(x)$.
  - **Homogeneous:** $y' + a(x)y = 0$.
  - **General Solution:**
    - Find integrating factor $\mu(x) = e^{\int a(x) dx}$.
    - Solution: $y(x) = \frac{1}{\mu(x)} \left( \int \mu(x) b(x) dx + c \right)$.
  - **Cauchy-Lipschitz Theorem:** Guarantees existence and uniqueness of solutions with initial condition $y(x_0) = y_0$.

#### Second Order Linear Equations (Constant Coefficients)
- **Form:** $a y'' + b y' + c y = f(x)$, $a \neq 0$.
- **Homogeneous:** $a y'' + b y' + c y = 0$.
- **Characteristic Equation:** $a r^2 + b r + c = 0$.
  - **Distinct Real Roots:** $y(x) = \alpha e^{r_1 x} + \beta e^{r_2 x}$.
  - **Double Root:** $y(x) = (\alpha + \beta x) e^{r_0 x}$.
  - **Complex Roots:** $y(x) = e^{\lambda x} (\alpha \cos(\mu x) + \beta \sin(\mu x))$.
- **General Solution:** Sum of general solution to homogeneous equation and a particular solution to the nonhomogeneous equation.
- **Variation of Constants:** Used to find particular solutions.

#### Physical Applications
- **Free Fall (No Friction):**
  - $a = g$, $v'(t) = g$, $v(t) = g t$ (if $v(0) = 0$).
  - $x'(t) = v(t)$, $x(t) = \frac{1}{2} g t^2$ (if $x(0) = 0$).
- **Parachutist (With Friction):**
  - $v'(t) = g - f v(t)$, $f$ is friction coefficient.
  - Solution: $v(t) = \frac{g}{f} + k e^{-f t}$, $k$ from initial condition.
- **Oscillator (Spring, No Damping):**
  - $m x'' + k x = 0$, $x(t) = A \cos(\omega t) + B \sin(\omega t)$, $\omega = \sqrt{\frac{k}{m}}$.
- **Oscillator (With Damping):**
  - $m x'' + f m x' + k x = 0$, $f$ is damping coefficient.
  - Solution depends on discriminant $f^2 - 4 k/m$.

---
## 📝 Notes
- Differential equations model many physical phenomena: motion, growth, decay, oscillations.
- Separable equations can be solved by integrating both sides after separating variables.
- Linear equations use integrating factors or variation of constants.
- The general solution to a linear equation is the sum of the homogeneous and particular solutions.
- Initial conditions are needed for unique solutions (Cauchy problem).
- Second order equations with constant coefficients are solved using the characteristic equation.
- Physical examples: free fall, parachutist (with friction), mechanical oscillator (spring, with/without damping).
