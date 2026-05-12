---
aliases:
  - Chapter_I
---
# Linear Forms, Dual Space
### Definitions 
##### 1.1
Let $E$ be a $K$ vector space. we call **Linear Form** of $E$ and note $E^*$ the vector space of linear forms in $E$. we type $E^* = \mathcal{L}(E,k)$ and $\phi \in E^*$ is the function $\phi:E \to K$ is an application such that $\forall (x,y) \in E^2$ and $\forall (\alpha,\beta) \in K^2$, $\phi(\alpha x + \beta y) = \alpha \phi(x) + \beta \phi(y)$.

### Propositions
##### 1.1 
let $n \in \mathbb{N}^*$.
- Let $(\lambda_{1},\dots,\lambda_{n}) \in K^n$. the application of $K^n$ in $K$ that gives each $x=(x_{1},\dots,x_{n}) \in K^n$. the scalar $\phi(x) = \sum_{1}^n \lambda_{j}x_{j}$, is a linear form in $K^n$.
- for all linear forms $\phi$ in $K^n$, there is a unique $(\lambda_{1},\dots,\lambda_{n}) \in K^n$ such that for all $x = (x_1,\dots, x_{n} ) \in K^n$, we have $\phi(x) = \sum_{1}^n \lambda_{j}x_{j}$.
##### 1.2
Let $E$ be a $k$-vector space of finite dimension. then its dual $E^*$ is a finite dimension and dim$E^*$ = dim $E$.
# Hyper Plans
## Definitions
##### 1.2
Let $E$ be $K$ vector space. we call a **Hyperplan** of $E$, the core of all linear forms in $E$  other that the null form, a part $H$ of $E$ is a hyperplan of $E$ if there is $\phi \in E\setminus {0}$ such that $H=Ker(\phi)$. we say that the relation $\phi(x) = 0$ is the equation of the hyperplan $H$.

### Propositions 
##### 1.2
let $H$ be a sub vector space of $E$:
- $H$ is a hyperplan of $E$.
- there is a vector line $D$ of $E$ such that $E = H \oplus D$.
- dim $H$ = dim $E$ - 1

# Dual Base
Let $E$ be a vector space of finite dimension, $n \ge 1$. 
### Propositions 
##### 3.1
Let $\mathcal{B} = (e_{j})_{j=1}^n$ be a base of $E$. the family of the coordinates $\mathcal{B}^* = (e_{i}^*)_{i=1}^n$ is a base of the dual space $E^*$, is called **dual base** of $\mathcal{B}$. and, for all $i,j \in [1,n]$, we have the relations of Kronecker :$$e_{i}^*(e_{j}) = \delta_{ij} = \begin{cases}
1 & i=j \\ 0 & i \ne j
\end{cases}$$
##### 3.2 
- if $\phi$ is linear form non null in $E$, there exists a vector $x \in E$ such that $\phi(x) = 1$.
- same but for $x$ instead of $\phi$.
##### 3.3
for all base of $E^*$ is the dual base of a unique base of $E$, called **Pre-dual basis**.
##### 3.4
Let $\mathcal{B_{1}, \mathcal{B_{2}}}$ be two bases of $E$, let $P$ be the passage matrix of $\mathcal{B_1}$ to $\mathcal{B_{2}}$. The passage matrix of $\mathcal{B_{1}^*}$ to $\mathcal{B_{2}^*}$ is ${}^tP$.
# Bi-dual of a vector space
### Definitions
##### 4.1
Let $E$ be a vector space. the dual of $E^*$, noted $E^{**}$ is called **Bi-dual** of $E$.$$\begin{aligned}
\Phi : E &\rightarrow E^{**} \\
x &\mapsto \tilde{x} : E^* \rightarrow K \\
&\quad\quad \varphi \mapsto \varphi(x)
\end{aligned}
$$
$\Phi$ is an isomorphism of vector space.