---
aliases:
  - Chapter_II
---
# magnetic induction field
## Lorentz Law
the expression of the force is : $$\vec{F} = q (\vec{E}+ \vec{v}\times \vec{B})$$ where $\vec{v}$ is the velocity and $\vec{B}$ is the **Magnetic induction field**.
$B$ is in **tesla** but sometimes we use **Gauss** (=$10^{-4}$ Tesla).
## Laplace Law
the set of charges in conductor in a section $S$ of length $l$ is teh force $$\vec{F} = l \vec{l}\times \vec{B}$$
## Biot and Savart Law
$$d\vec{B} = \frac{\mu_0}{4\pi} \frac{ld\vec{l}\times \vec{u}}{r^2}$$
with$\frac{\mu_0}{4\pi} = 10^{-7}$. and $\vec{B} = \int_c d\vec{B}$.

# Flux of $\vec{B}$ is conservative
from the Biot and Savart Law $div\vec{B} = \vec{\nabla}\vec{B}=0$.
and applying some more stuffs we can conclude at the end that it's conservative.

# Ampere Theorem
## Circulation of the magnetic field
$$
\begin{aligned}
dC &= \vec{B}.d\vec{M} \\
C &= \frac{\mu_0 l}{4\pi} \iint\frac{\vec{r}}{r^3}(d\vec{M}\times d\vec{l}) \\
C &= \mu_0 l \left(\frac{1}{4\pi}(\Omega - \Omega')\right)
\end{aligned}
$$
## integral
- if it's $n$ times in the positive sense and $p$ times in the negative sense $$\oint_\Gamma \vec{B}.d\vec{M} = \mu_0 (n-p) l$$
- if we started multiple circuits $$\oint_{\Gamma} \vec{B}.d\vec{M} = \sum_k \mu_0 \epsilon I_k$$
$\epsilon = + 1$ if it's positive, $\epsilon = -1$ if it's negative.
## Local form
$$\vec{rot\vec{B}} = \mu_0 \vec{j} \text{ Maxwell relationship}$$
## Symmetry Law 
- if the distribution is in a symmetry plan $\vec{B}$ is perpendicular to the plan.
- if the distribution have a symmetry axis $\Delta$ then : $\forall M \in \Delta; B(M)=0$.

# Potential vector $\vec{A}$ of the induction vector $\vec{B}$:
## Potential vector Notion 
$$\vec{B} = \vec{\nabla} \times \vec{A}$$
## Potential vector of induction vector
$$\vec{A} = \frac{\mu_0 l}{4 \pi} \int \frac{d\vec{l}}{r}$$
## Indeterminate of $\vec{A}$
$$\vec{\nabla}. \vec{A} = div \vec{A} = 0$$




























