---
aliases:
  - chapter_II
---

## 📚 Course Structure
- Section 1: **Electric Flux & Surfaces**
- Section 2: **Gauss's Theorem: Statement & Cases**

---
## 📐 Equations & Concepts
#### Electric Flux & Surfaces
- **Electric Flux through a Surface:**
  - The elementary flux of the electric field $\vec{E}$ through a surface $S$ is:
    $$
    d\Phi = \vec{E} \cdot d\vec{s}
    $$
    where $d\vec{s}$ is the oriented surface element (normal vector).
  - For a point charge $q$ at $O$, at distance $r$ from $M$:
    $$
    \vec{E}(M) = \frac{1}{4\pi\varepsilon_0} \frac{q}{r^2} \vec{u}_{OM}
    $$
    The elementary flux is:
    $$
    d\Phi = \vec{E}(M) \cdot d\vec{s} = \frac{q}{4\pi\varepsilon_0} \frac{\cos\theta\, ds}{r^2}
    $$
    $\theta$ is the angle between $\vec{E}$ and $d\vec{s}$.
  - **Solid Angle:**
    $$
    d\Omega = \frac{\cos\theta\, ds}{r^2}
    $$
    So, $d\Phi = \frac{q}{4\pi\varepsilon_0} d\Omega$
  - **Total Flux through Surface $S$:**
    $$
    \Phi = \int_S \vec{E} \cdot d\vec{s}
    $$
    For a closed surface around $q$ at $O$, the total solid angle is $4\pi$, so:
    $$
    \Phi = \frac{q}{\varepsilon_0}
    $$

- **Flux through a Sphere Centered on a Point Charge:**
  - On a sphere of radius $r$ centered at $q$:
    $$
    \Phi = \int_S \vec{E} \cdot d\vec{s} = \frac{q}{\varepsilon_0}
    $$
  - The flux is independent of the radius of the sphere.

- **Flux through Any Closed Surface:**
  - If the charge $q$ is inside the surface, the total flux is $\frac{q}{\varepsilon_0}$.
  - If $q$ is outside, the total flux is $0$.
  - If $q$ is on the surface, the flux is $\frac{q}{2\varepsilon_0}$ (not always, but for symmetric cases).

#### Gauss's Theorem: Statement & Cases
- **Gauss's Theorem (Point Charges):**
  - The net electric flux out of a closed surface $S$ is equal to the algebraic sum of the enclosed charges divided by $\varepsilon_0$:
    $$
    \oint_S \vec{E} \cdot d\vec{s} = \frac{\sum q_{\text{int}}}{\varepsilon_0}
    $$
  - The result does not depend on the position of the charges inside or the presence of charges outside $S$.

- **Gauss's Theorem (Continuous Distributions):**
  - For a continuous charge distribution inside $S$:
    $$
    \oint_S \vec{E} \cdot d\vec{s} = \frac{Q_{\text{int}}}{\varepsilon_0}
    $$
    - **Volume charge:** $Q = \int_V \rho_v dv$
    - **Surface charge:** $Q = \int_S \rho_s ds$
    - **Line charge:** $Q = \int_L \rho_l dl$
  - $V$, $S$, $L$ are the volume, surface, or line inside the closed surface $S$.

---
## 📝 Notes
- The electric flux through a closed surface depends only on the total charge enclosed.
- The flux is independent of the shape or size of the surface, as long as it is closed.
- Gauss's theorem is a powerful tool for calculating electric fields in cases with high symmetry (spheres, cylinders, planes).
- For charges outside the surface, their contribution to the total flux is zero.
