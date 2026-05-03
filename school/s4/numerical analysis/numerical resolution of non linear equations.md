---
aliases:
  - Chapter_IV
---
# Dichtomy Method
$$|x_n-c| \le \frac{b-a}{2^{n+1}}$$
# fixed point Method
## Definitions
##### 2.1
Let $F$ be the continuous function in an interval [a,b], with values in $[a,b]$. we say that $F$ is a contraction in $[a,b]$ if there's a $k$ in $]0,1[$ such that : $$|F(y)- F(x)| \le k |y-x|,  \forall x,y \in [a,b]$$
we say that $F$ contract in ration with $k$.
## Propositions
##### 2.1
the error estimation is $$|x_n - c| \le \frac{k^n}{1-k} |x_1 - x_0|$$
# Newton Method 
## Theorems 
##### 3.1
- **convergence**
	Newton method converges in a neighbor $V$ of $c$ with $x_0$ in $V$.
- **error estimation**
		$$|x_n - c| \le \left(\frac{M}{2m}^{2^n -1}\right)|x_0 -c|^{2^n}$$
	where $M = sup_V |f"|, m = inf_V|f'|$.

# secant method
## Theorems 
##### 4.1
we suppose that the function $f$ is a $\mathcal{C}^2$ then : 
the secant method converge in the neighbor $V$ of $c$ with $x_0$ in $V$ and the convergence is of order $p= \frac{1+\sqrt{5}}{2}$.

# False Law 




















































