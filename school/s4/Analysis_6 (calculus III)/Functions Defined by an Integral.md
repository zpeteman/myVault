---
aliases:
  - Chap_I
---
# Introduction
Let  $t \to f(x,t)$ be integral in $J$ such that $J, I \in \mathbb{R}$, for all $x \in I$ we have : $$F(x) = \int_J f(x,t)dt$$ we have two cases for this integral : 
- when the integral is said to be **proper integral**.
- when the integral is said to be **generalized integral**.

# Functions defined by a proper integral
in this section let $J=[a,b]$ and $I = ]\alpha, \beta[$ and $\alpha, \beta$ can be infinite.
### Theorems
##### 1.1: continuity
Let $f$ be a continuous in $I \times J$  then $F$ is continuous is $I$. then $\forall x_0, \lim_{x_0} F(x) =F(x_0)$ which gives us: $$\lim_{x_0} \int_J f(x,t)dt = \int_J \lim_{x_0} f(x,t)dt$$
##### 1.2: deferential
Let the partial def of $f$ be $\frac{\partial f}{\partial x} (x,t)$ and it's continuous in $I \times J$. Then the function $F$ is a $\mathcal{C}^1$ in $I$. And we have $$F'(x) = \int_a^b \frac{\partial f}{\partial x}(x,t)dt$$ The same for higher order def.
##### 1.3: Integral
Let $f$ be continuous in $I \times J$ Then $F$ is integral on $I$ and on $a$ $$\int_{\alpha}^{\beta} \left(\int_a^b f(x,t)\right) dx = \int_a^b \left( \int_{\alpha}^{\beta}f(x,t)\right) dx$$ 

# Functions Defined using a generalized integral
now Let $J = ]a,b[$ be not bounded, and the function $t\to f(x,t)$ not bounded in the neighbor of $a$ and $b$.
### Theorems
##### 1.4: continuity 
let $f$ be continuous and there's a function $g: t \in J \to \mathbb{R}^+$ such that $\int_a^b g(t)dt$ converges and $\forall x \in ]\alpha, \beta[$ $$\int_a^b |f(x,t)| \le \int_a^b g(t)dt$$ then $F$ is continuous in $I$.
we say that the integral $\int_a^b f(x,t) dt$ normal convergence.
##### 1.5: def
we must have : 
- $\int_a^b f(x,t)dt$ exist for $x_0 \in I$
- $\frac{\partial f}{\partial x} (x,t)$ is continuous if $I \times J$.
- $\int_a^b \frac{\partial f}{\partial x} (x,t)dt$ is normal convergent in $I$.
Then we can say that $F$ is a class $\mathcal{C}^1$ is $I$. $$F'(x) = \int_a^b \frac{\partial f}{\partial x}(x,t)dt$$ and the same is true for higher numbers.
##### 1.6
if $f(x,t)$ does converges normally then $F(x)$ have an integral.
























