---
aliases:
  - Chapter_3
---
# Existence and unity of the interpolation polynomial
## Theorems
##### 1.1
the polynomial $P_n$ interpolates $f$ at the points $x_0,x_1 , \dots , x_n$ exist and unique.

# Lagrage interpolation method
## Definitions
##### 2.1
the family $L_0,\dots, L_n$ called Lagrange associated to the points $x_0,x_1,\dots x_n$.
##### 2.2
the polynomial interpolation of Lagrange of the function $f$ at the points $x_0, \dots , x_n$ is defined by $P_n(x) = \sum_0^n f(x_i)L_i(x)$.
## Propositions 
##### 2.1
Let $L_i(x) = \Pi_{{j=O}_{j \ne i}}^n \frac{x-x_j}{x_i-x_j}$.
- $L_i$ is a polynomial of degree equal to $n$.
- $L_i (x_j) = \delta_{ij}$ where $\begin{cases}0 , j \ne i \\ 1, j=i\end{cases}$
- the family $L_0,\dots, L_n$ is a base of the set of polynomials of degree less than $n$.

# Newton interpolation of Polynomials
## Definitions
##### 3.1
let $f$ a function defined is $[a,b]$ where we know the values of $f(x_i)$ 
$$
\begin{array}{|c|c|c|}
\hline \text{Ordre} & \text{diffrenece} & \text{Definition} \\
\hline 0 & f[x_i] & f(x_i) \\
\hline 1 & f[x_i, x_j] & \displaystyle \frac{f(x_j) - f(x_i)}{x_j - x_i} \\
\hline 2 & f[x_i, x_j, x_k] & \displaystyle \frac{f[x_j, x_k] - f[x_i, x_j]}{(x_k - x_i)} \\
\hline \vdots & \vdots & \vdots \\
\hline n & f[x_0, x_1, \dots, x_{n-1}, x_n] & \displaystyle \frac{f[x_1, \dots, x_n] - f[x_0, \dots, x_{n-1}]}{x_n - x_0} \\
\hline
\end{array}
$$
##### 3.2
the newton interpolation of Newton of the function $f$ at the points $x_0,\dots, x_n$ is the polynomial of degree $n$ defined by $$P(x)= f(x_0) + (x-x_0)f[x_0,x_1] + \dots + (x-x_0)\dots(x-x_{n-1})f[x_0,\dots,x_n]$$

## Propositions
##### 3.1
- $f[x_i,x_j]=  \frac{f(x_i)}{x_i - x_j} + \frac{f(x_j)}{x_j - x_i}$.
- in general : $$f[x_0,\dots, x_m] = \sum_0^m \frac{f(x_i)}{\Pi_{{j=o}_{j \ne i}} (x_i - x_j)}$$
##### 3.2
the polynomial interpolation of Lagrange and the Newton polynomial interpolation are the identical.

# Error interpolation
## Theorems 
##### 4.1
we suppose that $f$ is a $\mathcal{C}^{m+1}([a,b])$ then : 
$\forall x \in [a,b]$ there exists $\epsilon_x$ in the smallest interval $$E_n(x) = \frac{1}{(n+1)!} \pi_n(x)f^{n+1}(\epsilon_x)$$ where $\pi_n(x)=\Pi_0^n(x-x_i)$.
if $f\in C^{n+1}([a,b])$ then $$|E_n(x) \le \frac{M_{n+1}|\pi_n(x)|}{(n+1)!}$$
where $M_{n+1} = max_{[a,b]}|f^{(n+1)}|$.
























