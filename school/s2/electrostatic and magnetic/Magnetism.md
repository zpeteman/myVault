---
aliases:
  - chapter_V
---

## 📚 Course Structure
- Section 1: **Magnetism & Magnetic Field**
- Section 2: **Magnetic Force (Lorentz & Laplace)**
- Section 3: **Magnetic Field from Moving Charges & Currents**
- Section 4: **Magnetic Flux & Conservation**
- Section 5: **Ampère's Theorem & Calculation Methods**

---
## 📐 Equations & Concepts
#### Magnetism & Magnetic Field
- **Magnets:** Have north and south poles; like poles repel, unlike attract. Magnetic effects are strongest at the poles.
- **Magnetic Field ($\vec{B}$):** Region where a magnetic pole experiences a force. Field lines exit the north pole and enter the south pole. Measured in tesla (T).

#### Magnetic Force (Lorentz & Laplace)
- **Lorentz Force:**
  - On a charge $q$ moving with velocity $\vec{v}$ in a magnetic field $\vec{B}$:
    $$
    \vec{F} = q \vec{v} \times \vec{B}
    $$
  - Direction: Perpendicular to both $\vec{v}$ and $\vec{B}$ (right-hand rule).
  - Magnitude: $F = q v B \sin \theta$
  - No force if the charge is at rest or $\vec{v}$ is parallel to $\vec{B}$.
- **Laplace Force:**
  - On a wire of length $\ell$ carrying current $I$ in $\vec{B}$:
    $$
    \vec{F} = I \vec{\ell} \times \vec{B}
    $$
  - Direction: Perpendicular to both the wire and $\vec{B}$ (right-hand rule).
  - Magnitude: $F = I \ell B \sin \theta$

#### Magnetic Field from Moving Charges & Currents
- **Single Moving Charge:**
  - At point $M$ due to charge $q$ moving at $\vec{v}$:
    $$
    \vec{B}(M) = \frac{\mu_0}{4\pi} \frac{q \vec{v} \times \vec{u}}{r^2}
    $$
    where $\mu_0$ is the vacuum permeability, $\vec{u}$ is the unit vector from the charge to $M$, $r$ is the distance.
- **Many Moving Charges (Continuous Distribution):**
  - For a volume with charge density and average velocity:
    $$
    \vec{B}(M) = \frac{\mu_0}{4\pi} \int_V \frac{\rho \vec{v} \times \vec{u}}{r^2} dv
    $$
- **Biot-Savart Law (Current Element):**
  - For a current $I$ in a wire element $d\vec{\ell}$:
    $$
    d\vec{B}(M) = \frac{\mu_0}{4\pi} \frac{I d\vec{\ell} \times \vec{u}}{r^2}
    $$
  - Total field: $\vec{B}(M) = \frac{\mu_0}{4\pi} \int_C \frac{I d\vec{\ell} \times \vec{u}}{r^2}$

#### Magnetic Flux & Conservation
- **Magnetic Flux through Surface $S$:**
  $$
  \Phi = \int_S \vec{B} \cdot d\vec{S}
  $$
- **Conservation of Magnetic Flux:**
  - For any closed surface, $\Phi = 0$ (no magnetic monopoles).
  - All field lines entering a closed surface also exit it.

#### Ampère's Theorem & Calculation Methods
- **Ampère's Theorem:**
  - The circulation of $\vec{B}$ around a closed curve $C$ equals $\mu_0$ times the total current $I$ passing through the surface bounded by $C$:
    $$
    \oint_C \vec{B} \cdot d\vec{\ell} = \mu_0 I_{\text{enc}}
    $$
  - Use symmetry to choose $C$ for easy calculation.
- **Calculation Methods:**
  - **Biot-Savart:** For filiform circuits, sum vector contributions.
  - **Flux Conservation:** Use when field is known elsewhere.
  - **Ampère's Theorem:** Use for symmetric current distributions.

---
## 📝 Notes
- Magnetic field lines always form closed loops; there are no isolated magnetic charges.
- Lorentz force acts only on moving charges and is perpendicular to both velocity and field.
- Laplace force describes the force on a current-carrying wire in a magnetic field.
- Biot-Savart law allows calculation of $\vec{B}$ from currents; Ampère's theorem relates field circulation to enclosed current.
- Use symmetry to simplify field calculations; flux conservation highlights the difference from electrostatics.
