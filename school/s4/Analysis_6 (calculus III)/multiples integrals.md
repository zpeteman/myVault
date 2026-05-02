---
aliases:
  - Chap_II
---
# Pavable and Squarable Sets of $\mathbb{R}^n$
## Pabale of $\mathbb{R}^n$
### Definitions
##### 2.1 
a paving is a part equal to the interval product $P = \Pi_{1 \le i \le n} [a_i;b_i]$, and $\mu(P) = \Pi_{1 \le i \le n}(b_i -a_i)$ is called the mesure of the paving $P$.
##### 2.2
the union of a finite number of paving is a paving such that $P_i \cap P_j =  \emptyset$ then we have $\mu(P) = \sum_{1 \le i \le k}(P_i)$.

## Squarable Sets of $\mathbb{R}^n$
### Definitions 
##### 2.3
Let $A$ be a party we note $m^+(A)$ the lower bound and $m^-(A)$ the upper bound of all pavings containing $A$, we say that $A$ is a Squarable Set if and only if $m^+(A)=m^-(A)$ and the common value of the two boundes si called the mesure of $A$ and noted $\mu(A)$.

### Propositions
##### 2.1
Let $A, B$ be two squarable sets then : 
- the parts or $A$ and $\bar{A}$ are squarable sets  and we have $\mu(A) = \mu(\bar{A})$.
- $\mu(A)+\mu(B) = \mu(A \cap B) + \mu(A \cup B)$.

# Multiple integral of a bounded function
## Darboux Sums
- $$s(\delta) = \sum_{i\in I} \mu(A_i)m_i, S(\delta) = \sum_{i\in I} \mu(A_i)M_i $$ where the reals $m_i$ and $M_i$ are the sub born and the up born of the function $f$ is the part $A_i$.
- $f$ is integral in $A$ if $inf_{\Delta} S(\delta) = sup_{\Delta} s(\delta)$. where $\Delta$ is the set of all subdivisions of the squarable set inside the $A$, the common value of the boundes is called the **multiple integral** of $f$ in $A$ is noted $\int_A f d\mu$.
## Case of continuous functions
alll continuous function in squarable set does admet an integral.
# Proprieties of multiple integral
## Theorems
##### 2.2
$$\int_{A\cup B} f d\mu = \int_A f d\mu + \int_B f d\mu$$
##### 2.3
$$\int_A \alpha f + \beta g  d\mu = \alpha \int_A f d\mu + \beta \int_A g d\mu$$
$$\int_A f d\mu \le \int_A g d\mu \text{ if } f \le g$$
$$\left|\int_A f d\mu \right| \le  \int_A |f| d\mu$$
# Technics of calculation
## Fubini formula for Multiple integrals (double integrals as a simple example)
### Propositions
##### 2.2
Let $P = \Pi_{1 \le i \le n}[a_i;b_i]$ and $f: P \to \mathbb{R}$ which gives us $f(x) = \Pi_{1\le i \le n} f_i(x)$ then : $$\int_P f(x_1,x_2,\dots,x_n) dx_1dx_2\dots dx_n = \Pi_{1\le i \le n} \left(\int_{a_i}^{b_i}f_i(x_1,x_2,\dots,x_n)dx_i\right)$$
##### 2.3
$$\iint_D f(x,y) dxdy = \int_a^b  \left( \int_{\phi(x)}^{\psi(x)} f(x,y) dy \right)dx$$