---
aliases:
  - Chapter_II
---
# introduction
$$\begin{aligned}
Ax&= b \\
(M-N)x&=b \\
\implies 
&\begin{cases}
x_0 \in \mathbb{R}^n \\
Mx_{p+1} = Nx_p + b, \forall p \in \mathbb{N}
\end{cases}
\end{aligned}$$
which gives us the algorithm : $$\begin{cases}
x_0 \in \mathbb{R}^n \\
x_{p+1} = M^{-1}Nx_p + M^{-1}b,\forall p \in \mathbb{N}
\end{cases}$$
The matrix $M^{-1}N$ is called the iterative matrix.

# Jacobi methods, Gauss-Seidel and Method of relaxation
Let $A = D - E - F$ such that $D$ is diagonal
Now to solve the system $My = Ny + b$ we do : 
## Jacobi method
let $M = D, N = E + F$  then $$(x_{p+1})_i=(x_p)_i + \frac{1}{a_{ii}} \left(b_i - \sum_1^n a_{ij} (x_p)_j\right)$$ for $i = 1, \dots , n$.
## Gauss-Seidel method
let $M = D-E, N=F$
$M$ is a triangular matrix. $$\begin{aligned}
(x_{p+1})_1 &= (x_p)_1 + \frac{1}{a_{11}}\left(b_1 - \sum_1^n a_{1j}(x_p)_j\right) \\
(x_{p+1})_i &= (x_p)_i + \frac{1}{a_{ii}}\left(b_i - \sum_1^{i-1} a_{ij}(x_{p+1})_j - \sum_i^n a_{ij}(x_p)_j\right)
\end{aligned}$$
## Relaxation Method
Let $M = \frac{1}{\omega}D -E, N = \frac{1}{\omega}D - D + F$
$$\begin{aligned}
(x_{p+1})_1 &= (x_p)_1 + \frac{\omega}{a_{11}}(b_1 - \sum_1^n a_{1j}(x_p)_j) \\
(x_{p+1})_i &= (x_p)_i + \frac{\omega}{a_{ii}}(b_i - \sum_1^{i-1} a_{ij}(x_{p+1})_j - \sum_i^n a_{ij}(x_p)_j)
\end{aligned}$$
# convergence of iterative methods
## Definitions
##### 3.1
iterative methods are said to be convergent if, for all given initial $x_0$, the sequence $(x_p)$ define by $Mx_{p+1}=Nx_p + b (p\in \mathbb{N})$ converges to a solution $x$ of the linear system $Ax=b$.  
##### 3.2
Let $N$ be the norm of $\mathbb{K}^n$. we call the matrix norm $N$ the application $||.||$ define in a set of matrix $\mathcal{M}_n(\mathbb{K})$ with $||A|| = max_{x\in \mathbb{K}^n \setminus {0}} \frac{N(Ax)}{N(x)}$.
##### 3.3
the matrix $A$ is said to be diagonal by a line if : $|a_{ii}| > \sum_{j \ne i} |a_{ij}| , \forall i = 1,\dots, n$.
the matrix $A$ is diagonal by a column if : $|a_{ii}| > \sum_{j \ne i} |a_{ji}|, \forall i = 1, \dots , n$.

## Propositions
##### 3.1
Let $A$ be a $n$ order matrix, then :
- case where $N = || ||_1 : ||A||_1 = max_j \sum_1^n |a_{ij}|$.
- case  when  $N = ||||_{\infty}: ||A||_{\infty} = max_i \sum_1^n|a_{ij}|$.
- case when $N = ||||_2 : ||A||_2 = \sqrt{\rho (A^* A)}$.
$A^* = \bar{A}^T$ and $\rho$ is the radius of the spectral, $\rho(A) = max {|\lambda| , \lambda \text{ is the eignevalue of }A}$ 
- if the matrix $A$ is symmetrical then $||A||_2 = \rho(A)$.
##### 3.2
Let $B$ be a matrix in $\mathcal{M}_n (\mathbb{K})$: 
- $\lim_{\infty} B^p = 0$
- $\lim_{\infty} B^p y = 0, \forall y \in \mathbb{K}^n$
- $\rho(B) < 1$
- there's a norm where $||B|| < 1$
##### 3.3
the relaxation method diverges if $\omega \notin [0,2]$.

## Theorems
##### 3.1
if $||M ^{-1} N|| < 1$ then the iterative method converges.
##### 3.2
if $\rho(M^{-1}N) < 1$ then the iterative method converges.
##### 3.3
if the matrix $A$ is diagonal then the Jacobi method converges.
##### 3.4
if the matrix $A$ is strictly diagonal then the Gauss-Seidel converges.
##### 3.5
- if the matrix $A$ is strictly diagonal then the relaxation method converges if $0 < \omega \le  1$.
- if the matrix $A$ is symmetrical and positively defined then the relaxation method converges if $0 < \omega < 2$.
































































