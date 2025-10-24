---
aliases:
  - Chaptre_0
---
## 📚 Course Structure
- Section 1: **Torsors and Velocity Fields**
- Section 2: **Kinetic Torsor**
- Section 3: **Dynamic Torsor**
- Section 4: **Kinetic Energy**
- Section 5: **Forces and Fundamental Principle of Dynamics**
- Section 6: **Power of External Forces**

---
## 📐 Equations & Concepts

#### Torsors and Velocity Fields:
- **Reduction Elements of a Torsor:**
  - $\tau(A) = [\mathbf{r}, \mathbf{M}(A)]$
  - Moment transfer: $\mathbf{M}(A) = \mathbf{M}(B) + \mathbf{r} \wedge \mathbf{AB}$
- **Velocity Torsor:**
  - $\tau_v (P; S/R_0) = [\boldsymbol{\omega}_{S/R}, \mathbf{V}(P \in S/R_0)]$
  - Composition of rotations: $\boldsymbol{\omega}_{R_s/R} = \boldsymbol{\omega}_{R_s/R_2} + \boldsymbol{\omega}_{R_2/R_1} + \boldsymbol{\omega}_{R_1/R_0}$
  - Velocity field: $\mathbf{V}(P \in S/R_0) = \mathbf{V}(M \in S/R_0) + \boldsymbol{\omega}_{S/R_0} \wedge \mathbf{GP}$
- **Non-Slip Condition:**
  - $\mathbf{V}_g(I) = \mathbf{V} (I \in S_1 / R) - \mathbf{V} (I \in S_2 / R) = 0$

#### Kinetic Torsor:
- **Reduction Elements:**
  - $\tau_c (A; S / R_0) = [\mathbf{P} (S / R_0) ; \boldsymbol{\sigma} (A; S / R_0)]$
- **Center of Mass Theorems:**
  - Theorem I: $\mathbf{P} (S / R_0) = m \mathbf{V} (G \in S / R_0)$
  - Theorem II: $\boldsymbol{\sigma} (G; S / R_0) = \mathbf{J} (G; S / R_0) \cdot \boldsymbol{\omega}_{S / R_0}$
- **Koenig's Theorems:**
  - Theorem II: $\boldsymbol{\sigma} (O; S / R_0) = \mathbf{J} (G, S) \cdot \boldsymbol{\omega}_{S / R_0} + m \mathbf{O G} \wedge \mathbf{V} (G \in S / R_0)$
  - Theorem I (Inertia): $\mathbf{J} (O, S) = \mathbf{J} (O; [G]) + \mathbf{J} (G, S)$

#### Dynamic Torsor:
- **Reduction Elements:**
  - $\tau_D (A; S/R_0) = [\mathbf{S}(S/R_0); \mathbf{D}(A; S/R_0)]$
  - Dynamic resultant: $\mathbf{S}(S/R_0) = m \mathbf{a}(G \in R_s/R_0)$
  - Dynamic moment: $\mathbf{D}(A; S/R_0) = \left( \frac{d\boldsymbol{\sigma} (A; S/R_0)}{dt} \right)_{R_0} + m\mathbf{V}(A/R_0) \wedge \mathbf{V}(G/R_0)$
- **Special Cases:**
  - Fixed point A: $\mathbf{D}(A; S/R_0) = \left( \frac{d\boldsymbol{\sigma} (A; S/R_0)}{dt} \right)_{R_2} + \boldsymbol{\omega}_{R_2/R_0} \wedge \boldsymbol{\sigma} (A; S/R_0)$

#### Kinetic Energy:
- **Koenig's Theorem IV:**
  - $E_c(S/R_0) = \frac{1}{2}m\mathbf{V}^2 (G; S/R_0) + \frac{1}{2}\boldsymbol{\omega}_{S/R_0} \cdot \boldsymbol{\sigma} (G; S/R_0)$
  - Alternative form: $2E_c(S/R_0) = \tau_c(G; S/R_0) \cdot \tau_V(G; S/R_0)$
  - General point A: $2E_c(S/R_0) = \tau_c(A; S/R_0) \cdot \tau_V(A; S/R_0)$

#### Forces and Fundamental Principle of Dynamics:
- **External Force Torsor:**
  - $\tau_F(O; S/R_0) = [\mathbf{F}(S/R_0); \mathbf{M}(O; S/R_0)]$
  - Resultant force: $\mathbf{F}(S/R_0) = \sum_i \mathbf{F}_i$
  - Resultant moment: $\mathbf{M}(A; S/R_0) = \sum_{P_i \in S} \mathbf{OP}_i \land \mathbf{F}_i$
- **Fundamental Principle:**
  - $\tau_D(S/R_0) = \tau_F^{ext}(S/R_0)$
  - Dynamic resultant: $m\mathbf{a}(M/R_0) = \sum_i \mathbf{F}_i^{ext}$
  - Angular momentum theorem: $\left( \frac{d\boldsymbol{\sigma} (O; S/R_0)}{dt} \right)_{R_0} = \mathbf{M}_{F^{ext}} (O; S/R_0)$

#### Power of External Forces:
- **Instantaneous Power:**
  - $P(t; S/R_0) = (\tau_v (A; S/R_0); \tau_F^{ext} (A; S/R_0))$
  - $P(t; S/R_0) = \mathbf{F}_i \cdot \mathbf{V}(A \in S/R) + \boldsymbol{\omega}_{S/R} \cdot (\mathbf{AM}_i \wedge \mathbf{F}_i)$
- **Work:**
  - $\mathbf{W}(t_0, t_1, S/R) = \int_{t_0}^{t_1} P(t; S/R) dt$

---
## 📝 Notes
- Torsors are used to represent physical quantities (velocity, kinetic, dynamic, forces) in a compact form.
- The choice of point A can simplify calculations significantly.
- Internal forces do not appear in the external force torsor.
- Koenig's theorems relate quantities at the center of mass to those at other points.
- The non-slip condition is crucial for rolling without slipping problems.
- The power of forces helps determine work, especially for non-conservative forces.