---
aliases:
  - chapter_I
---

## 📚 Course Structure
- Section 1: **Electrization & Charge Properties**
- Section 2: **Coulomb's Law & Applications**
- Section 3: **Electric Field & Distributions**

---
## 📐 Equations & Concepts
#### Electrization & Charge Properties
- **Electrization:**
  - By contact: touching a neutral body with a charged one.
  - By influence: bringing a charged body near a neutral one, then removing it.
  - By sources: connecting to a battery or generator.
- **Conductors & Insulators:**
  - Insulators: Do not conduct charge (glass, dry air, plastic).
  - Conductors: Conduct charge easily (metals, humid air, water).
- **Charge Properties:**
  - Two types: positive and negative. Like charges repel, unlike attract.
  - Total charge is the sum of elementary charges.
  - Neutral bodies have equal amounts of opposite charges.
  - Charge is conserved and quantized: $q_e = 1.6021 \times 10^{-19}$ C.
  - Charge is invariant (does not depend on reference frame).
- **Continuous Charge Distributions:**
  - Volume: $\rho_v = \lim_{dv \to 0} \frac{dq}{dv}$, $Q = \int_V \rho_v dv$
  - Surface: $\rho_s = \lim_{ds \to 0} \frac{dq}{ds}$, $Q = \int_S \rho_s ds$
  - Line: $\rho_l = \lim_{dl \to 0} \frac{dq}{dl}$, $Q = \int_L \rho_l dl$

#### Coulomb's Law & Applications
- **Coulomb's Law:**
  - Two point charges $q_1$ and $q_2$ at distance $r$ exert a force:
    $$
    F = k \frac{q_1 q_2}{r^2}
    $$
    where $k = \frac{1}{4\pi\varepsilon_0}$, $\varepsilon_0 = 8.85 \times 10^{-12}$ C$^2$N$^{-1}$m$^{-2}$.
  - $F$ is repulsive if $q_1 q_2 > 0$, attractive if $q_1 q_2 < 0$.
- **Vector Form:**
  - For charges at $M_1$ and $M_2$, with unit vector $\vec{u}_{12}$ from $M_1$ to $M_2$:
    $$
    \vec{F}_{12} = k \frac{q_1 q_2}{r_{12}^2} \vec{u}_{12}
    $$
  - Action-reaction: $\vec{F}_{12} = -\vec{F}_{21}$.
- **Superposition Principle:**
  - For multiple charges, total force on $q$ is the vector sum of forces from each charge.
  - For continuous distributions (volume, surface, line):
    - Volume: $d\vec{F}_{PM} = k \frac{dq_P q}{r_{PM}^2} \vec{u}_{PM}$, $\vec{F}_M = \int_V d\vec{F}_{PM}$
    - Surface: $d\vec{F}_{PM} = k \frac{dq_P q}{r_{PM}^2} \vec{u}_{PM}$, $\vec{F}_M = \int_S d\vec{F}_{PM}$
    - Line: $d\vec{F}_{PM} = k \frac{dq_P q}{r_{PM}^2} \vec{u}_{PM}$, $\vec{F}_M = \int_L d\vec{F}_{PM}$

#### Electric Field & Distributions
- **Electric Field Definition:**
  - The field at $M$ due to charges $q_i$ at $M_i$:
    $$
    \vec{E}_M = \frac{\vec{F}_M}{q}
    $$
    $$
    \vec{E}_M = \sum_i k \frac{q_i}{r_{iM}^2} \vec{u}_{iM}
    $$
  - SI unit: N/C or V/m.
- **Field of a Point Charge:**
  - At distance $r$ from $q$:
    $$
    \vec{E}_M = k \frac{q}{r^2} \vec{u}_r
    $$
  - Radial, spherically symmetric, direction depends on sign of $q$.
- **Field of Multiple Charges:**
  - Sum the fields from each charge.
- **Field Lines & Tubes:**
  - Field lines: curves tangent to $\vec{E}$ at each point, oriented in the direction of $\vec{E}$.
  - Field tubes: surfaces formed by field lines from a closed contour.
  - Uniform field: field lines are parallel, tubes are cylinders.
- **Field from Continuous Distributions:**
  - Volume: $\vec{E}_M = \int_V k \frac{dq_P}{r_{PM}^2} \vec{u}_{PM}$
  - Surface: $\vec{E}_M = \int_S k \frac{dq_P}{r_{PM}^2} \vec{u}_{PM}$
  - Line: $\vec{E}_M = \int_L k \frac{dq_P}{r_{PM}^2} \vec{u}_{PM}$

---
## 📝 Notes
- Electrization can occur by contact, influence, or sources.
- Conductors allow charge movement; insulators do not.
- Charge is quantized, conserved, and invariant.
- Coulomb's law describes the force between two point charges; superposition extends it to many charges.
- The electric field is a vector field describing the force per unit charge.
- Field lines show the direction and strength of the field; tubes group field lines.
- For continuous charge distributions, integrate over the volume, surface, or line to find total field.
