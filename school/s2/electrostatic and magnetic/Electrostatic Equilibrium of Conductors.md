---
aliases:
  - chapter_IV
---

## 📚 Course Structure
- Section 1: **Electrostatic Equilibrium of Conductors**
- Section 2: **Multiple Conductors & Influence**
- Section 3: **Electrostatic Influence**
- Section 4: **Capacitance & Capacitors**
- Section 5: **Electrostatic Energy**

---
## 📐 Equations & Concepts
#### Electrostatic Equilibrium of Conductors
- **Conductors vs. Insulators:**
  - In conductors (e.g., metals), free electrons move easily; in insulators, electrons are tightly bound.
- **Electrostatic Equilibrium:**
  - A conductor is in equilibrium when free charges are at rest (no net movement).
  - In equilibrium, the electric field inside a conductor is zero ($\vec{E}_{\text{int}} = 0$), and any excess charge resides on the surface.
  - The potential is constant throughout the conductor and on its surface (the surface is an equipotential).
- **Charged Conductor:**
  - If a charge is placed on a conductor, it redistributes to reach equilibrium, with all excess charge on the surface.
  - For a hollow conductor, the same properties hold.
- **Electric Field Near Surface:**
  - Just outside a charged conductor, $E_{\text{surf}} = \frac{\sigma}{\varepsilon_0}$, where $\sigma$ is the surface charge density and $\varepsilon_0$ is the vacuum permittivity.
  - The field is normal to the surface.
- **Electrostatic Pressure:**
  - The pressure on the surface due to the field is $p = \frac{\varepsilon_0}{2} E_{\text{surf}}^2$.

#### Multiple Conductors & Influence
- **Corresponding Elements:**
  - For two conductors, charges on facing surface elements are equal and opposite.
- **Superposition Principle:**
  - The equilibrium state of a system of conductors is the sum of the equilibrium states for each conductor taken separately.
  - The potential and charge on each conductor are linear combinations of the potentials of all conductors.
- **Laplace's Equation:**
  - Outside conductors, the potential satisfies $\nabla^2 V = 0$ (Laplace's equation), with $V$ constant on each conductor.

#### Electrostatic Influence
- **Isolated Conductor in External Field:**
  - Placing a neutral conductor in an external field causes charge separation (induced charges), but the total charge remains zero.
  - The field inside remains zero; the surface charge redistributes to maintain equilibrium.
- **Conductor Near a Charged Conductor:**
  - A neutral conductor near a charged one acquires induced charges of opposite sign on the facing side.
  - If the neutral conductor is grounded, it can gain or lose net charge.
- **Total Influence:**
  - If a charged conductor is completely surrounded by another conductor, all field lines from the inner conductor end on the outer one (total influence).
- **Faraday Cage:**
  - A hollow, grounded conductor shields its interior from external electric fields.

#### Capacitance & Capacitors
- **Capacitance of a Conductor:**
  - $C = \frac{Q}{V}$, where $Q$ is the charge and $V$ is the potential relative to infinity.
  - For a sphere of radius $R$: $C = 4\pi\varepsilon_0 R$.
- **Capacitance of a System (Coefficients of Influence):**
  - For $n$ conductors: $Q_i = \sum_j C_{ij} V_j$, where $C_{ij}$ are coefficients of influence.
  - $C_{ii}$ is the self-capacitance; $C_{ij}$ ($i \neq j$) are mutual coefficients.
- **Capacitor:**
  - Two conductors (plates) with charges $+Q$ and $-Q$ and potentials $V_1$, $V_2$.
  - Capacitance: $C = \frac{Q}{V_1 - V_2}$.
- **Capacitors in Parallel:**
  - $C_p = C_1 + C_2 + \cdots + C_n$
- **Capacitors in Series:**
  - $\frac{1}{C_s} = \frac{1}{C_1} + \frac{1}{C_2} + \cdots + \frac{1}{C_n}$

#### Electrostatic Energy
- **Energy of a Point Charge:**
  - $U = q V_M$, where $V_M$ is the potential at point $M$.
- **Energy of a Charged Conductor:**
  - $U = \frac{1}{2} Q V = \frac{1}{2} C V^2 = \frac{Q^2}{2C}$
- **Energy of a System of Conductors:**
  - $U = \frac{1}{2} \sum_i Q_i V_i$
- **Energy of a Capacitor:**
  - $U = \frac{1}{2} C (V_1 - V_2)^2$
- **Energy Density:**
  - For a continuous charge distribution: $u = \frac{1}{2} \varepsilon_0 E^2$
  - Total energy: $U = \int_{\text{all space}} \frac{1}{2} \varepsilon_0 E^2 dv$

---
## 📝 Notes
- In electrostatic equilibrium, the field inside a conductor is zero and the surface is an equipotential.
- Excess charge on a conductor resides on its surface.
- Capacitance depends only on geometry and the medium.
- The Faraday cage effect shields the interior from external fields.
- The energy stored in a capacitor or system of conductors can be calculated from charge and potential.
- Energy is distributed in the electric field throughout space, not just on the conductors.
