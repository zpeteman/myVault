---
aliases:
  - chapter_III
---

## 📚 Course Structure
- Section 1: **Potential from Point Charges**
- Section 2: **Potential from Multiple Charges & Distributions**
- Section 3: **Equipotential Surfaces**
- Section 4: **Electrostatic Work & Potential Difference**
- Section 5: **Field-Potential Relations & Maxwell Equations**

---
## 📐 Equations & Concepts
#### Potential from Point Charges
- **Definition:** The electric potential at point $M$ at distance $r$ from charge $q$ is:
  $$
  V(M) = \frac{1}{4\pi\varepsilon_0} \frac{q}{r}
  $$
  - SI unit: Volt (V).
  - Not defined at $r = 0$ (on the charge).
  - By convention, $V = 0$ at infinity.
- **Potential Difference:**
  - The difference $V_A - V_B$ between points $A$ and $B$ is the work per unit charge to move from $A$ to $B$.
  - For a closed path, the total circulation is zero: the field is conservative.

#### Potential from Multiple Charges & Distributions
- **Superposition:**
  - For several point charges $q_i$ at distances $r_i$ from $M$:
    $$
    V(M) = \sum_i \frac{1}{4\pi\varepsilon_0} \frac{q_i}{r_i}
    $$
- **Continuous Distributions:**
  - Volume: $V(M) = \frac{1}{4\pi\varepsilon_0} \int_V \frac{\rho_v dv}{r_{PM}}$
  - Surface: $V(M) = \frac{1}{4\pi\varepsilon_0} \int_S \frac{\rho_s ds}{r_{PM}}$
  - Line: $V(M) = \frac{1}{4\pi\varepsilon_0} \int_L \frac{\rho_l dl}{r_{PM}}$

#### Equipotential Surfaces
- **Definition:** Surfaces where $V$ is constant.
  - For a point charge, equipotentials are spheres centered on the charge.
  - For two charges, equipotentials are more complex surfaces.
- **Field Lines:** Always orthogonal to equipotential surfaces.

#### Electrostatic Work & Potential Difference
- **Work by Electric Force:**
  - For a charge $q$ moving from $A$ to $B$:
    $$
    W_{AB} = q (V_A - V_B)
    $$
  - The work depends only on the endpoints, not the path.
- **Volt Definition:** 1 Volt is the potential difference when moving 1 Coulomb requires 1 Joule of work.

#### Field-Potential Relations & Maxwell Equations
- **Relation between Field and Potential:**
  - In Cartesian coordinates:
    $$
    \vec{E} = -\nabla V
    $$
    $$
    E_x = -\frac{\partial V}{\partial x},\quad E_y = -\frac{\partial V}{\partial y},\quad E_z = -\frac{\partial V}{\partial z}
    $$
  - In cylindrical and spherical coordinates, similar gradient relations apply.
- **Gauss's Theorem (Local Form):**
  - $$
    \nabla \cdot \vec{E} = \frac{\rho}{\varepsilon_0}
    $$
  - The flux of $\vec{E}$ through a closed surface equals the enclosed charge over $\varepsilon_0$.
- **Curl of $\vec{E}$:**
  - $$
    \nabla \times \vec{E} = 0
    $$
  - The electric field is irrotational (conservative).
- **Poisson and Laplace Equations:**
  - $$
    \nabla^2 V = -\frac{\rho}{\varepsilon_0}
    $$
  - If $\rho = 0$, then $\nabla^2 V = 0$ (Laplace's equation).

---
## 📝 Notes
- The electric potential is a scalar function related to the electric field by $\vec{E} = -\nabla V$.
- Equipotential surfaces are always perpendicular to field lines.
- The work done by the electric field depends only on the initial and final points.
- Gauss's theorem and Maxwell's equations link the field and potential to charge distributions.
- Poisson's and Laplace's equations are key for solving potential problems in electrostatics.
