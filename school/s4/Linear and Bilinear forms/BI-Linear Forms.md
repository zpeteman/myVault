---
aliases:
  - Chapter_II
---
# Symmetric Bi-Linear Forms
### Definitions 
##### 1.1
is an application $\phi: E \times E \to \mathbb{K}$ is a **Bi-Linear form** in $E$ if :
- $\forall y \in E, \phi_{y} : x \to \phi(x,y)$ is a linear form in $E$. we also say that $\phi$ is linear in portion to the first place.
- $\forall x \in E, \phi_{x} : y \to \phi(x,y)$ is a linear form in $E$. we say also that $\phi$ is a linear in portion the the second place.
Let $\phi$ is a bi-linear form in $E,m,n \in \mathbb{N}, \alpha_{1},\dots,\alpha_{n} \in \mathbb{K}$, $$\phi \left(\sum_{i=1}^n \alpha_{i}x_{i} , \sum_{j=1}^m \beta_{j}y_{j} \right) = \sum_{i=1}^n \sum_{j=1}^m \alpha_{i}\beta_{j}\phi(x_{i},y_{j})$$
##### 1.2
- we call **symmetrical BI-linear form** in $E$ all bi-linear form $\phi : E \times E \to \mathbb{K}$ that verifies : $$\forall x,y \in E, \phi (x,y) = \phi(y,x)$$
- we call **anti-symmetrical bi-linear form** in $E$ all bi-linear form $\phi: E \times E \to \mathbb{K}$: $$\forall x, y \in E , \phi (x,y) = - \phi (y,x)$$
- we call **alternative bi-linear forms** in $E$ all bi-linear form $\phi: E \times E \to \mathbb{K}$: $$\forall x \in E, \phi (x,x) = 0$$

### Propositions
##### 1.1
- the set $\mathcal{B}\mathcal{L}(E)$ is a sub vector space of $\mathcal{F}(E \times E, \mathbb{K})$.
- the set $\mathcal{S}(E)$ is a sub vector space of the space $\mathcal{B}\mathcal{L}(E)$.
# Quadratic Form
### Definitions 
##### 2.1 
we call **quadratic form** in $E$ all application $q: E \to \mathbb{K}$ of the form $$q : x \to \phi(x,x)$$ where $\phi$ is a bi-linear form in $E$. in this case, we say that $q$ is a quadratic form associated to $\phi$.
##### 2.2
all $fq$ $q$ in $E$ is associated to a unique $fbs$ $\phi$ in $E$ called **Polar form** of $q$ and defined by $(c),(d),(e)$ of the propositions.
### Theorems
##### 2.1
if $q$ is a quadratic form in $E$, then there exists a unique symmetrical bi-linear form $\phi$ such that $q(x) = \phi(x,x)$ for all $x \in E$.

# Positive Form and defined Positives
we suppose that $\mathbb{K} = \mathbb{R}$. let $\phi$ is an $fbs$ in $E$ and $q$ is the associated quadratic form.
### Definitions 
##### 3.1
- we say that $\phi$, or $q$ is **positive**, if it's verified $$\forall x \in E, \phi(x,x) \ge 0$$
- we say that $\phi$ or $q$ is **defined positive**, if it verifies $$\forall x \in E\setminus {0} \phi(x,x) > 0$$