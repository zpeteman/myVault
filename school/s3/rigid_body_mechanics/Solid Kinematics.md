---
aliases:
  - chapter_III
---
## 📚 Course Structure
- Section 1: **Center of Mass (G)**
- Section 2: **Solid's Inertia Operator: $J(S)$**

---
## 📐 Equations & Concepts

### Center of Mass (G)
- **Definition and Formulas:**
    - The center of mass G (or center of inertia) is the **barycenter** of the solid's points $P$ weighted by their masses.
    - **Position Vector:**
      $$mOG=\int_{P\in S}OPdm(P)$$
      where $m$ is the total mass of $S$:
      $$m=\int_{P\in S}dm(P)$$
    - **In Barycentric Frame $R_G$ (origin G):**
      $$\int_{S}GPdm=0$$
    - **For Composite Solids ($S=S_1 \cup S_2$):**
      $$OG=\frac{(m_{1}OG_{1}+m_{2}OG_{2})}{m_{1}+m_{2}}$$
- **Types of Mass Distribution:**
    - **Volume:** $dm(P)=\rho(P)d^{3}v$
    - **Surface:** $dm(P)=\sigma(P)d^{2}s$
    - **Line:** $dm(P)=\lambda(P)dl$
    - **Note:** Uniform distributions mean $\rho$, $\sigma$, and $\lambda$ are constant.
- **Calculation Rules via Material Symmetries:**
    - **Rule 1: Point of Symmetry A:** If $A$ is a point of material symmetry, $G$ coincides with $A$.
      $$A \text{ point of symmetry} \Leftrightarrow G=A$$
    - **Rule 2: Axis of Symmetry $\Delta$:** If $\Delta$ is an axis of material symmetry, $G$ lies on $\Delta$.
      $$G \in \Delta$$
    - **Rule 3: Plane of Symmetry $\Pi$:** If $\Pi$ is a plane of material symmetry, $G$ lies in $\Pi$.
      $$G \in \Pi$$

---
### Solid's Inertia Operator: $J(S)$
- **Definition of the Inertia Operator:**
    - The inertia operator $J(C;S)$ at a point $C$ is defined by:
      $$u \rightarrow J(C;S) \cdot u = \int_{P \in S} CP \wedge (u \wedge CP) dm$$
- **Properties and Inertia Matrix:**
    - $J(O;S)$ is a **linear symmetric operator**.
    - It is represented by a $3 \times 3$ symmetric matrix:
      $$J = \begin{pmatrix} A & -F & -E \\ -F & B & -D \\ -E & -D & C \end{pmatrix}$$
    - **Moments of Inertia (Diagonal):** Moments with respect to axes $OX, OY, OZ$.
      $$A = J_{xx} = \int_{S}(y^{2}+z^{2})dm$$
      $$B = J_{yy} = \int_{S}(x^{2}+z^{2})dm$$
      $$C = J_{zz} = \int_{S}(x^{2}+y^{2})dm$$
    - **Products of Inertia (Off-Diagonal):**
      $$F = -J_{xy} = \int_{S}xy~dm$$
      $$E = -J_{xz} = \int_{S}xz~dm$$
      $$D = -J_{yz} = \int_{S}yz~dm$$
- **Moment of Inertia with Respect to an Axis $\Delta=(O, u)$:**
    $$J_{\Delta} = u \cdot J(O) \cdot u$$
    - In coordinates $(u = \alpha X + \beta Y + \gamma Z)$:
      $$J_{\Delta}=A\alpha^{2}+B\beta^{2}+C\gamma^{2}-2D\beta\gamma-2E\alpha\gamma-2F\alpha\beta$$
- **Principal Axes and Diagonalization:**
    - The matrix $J(O)$ is **diagonalizable**.
    - The diagonal form $D(O)$ contains the **principal moments of inertia** $\lambda_{1}, \lambda_{2}, \lambda_{3}$.
- **Koenig's First Theorem (Inertia Operator):**
    - The inertia operator at point $O$ equals the sum of the operator at the center of mass $G$ and the operator at $O$ of a particle of mass $m$ at $G$.
      $$J(O;S)=J(O;\{G\})+J(G;S)$$
- **Huygens' Theorem (Parallel Axes Theorem):**
    - The moment of inertia $J_{\Delta_O}$ about an axis $\Delta_O$ is related to the moment $J_{\Delta_G}$ about a parallel axis $\Delta_G$ passing through $G$ by:
      $$J_{\Delta_{O}}=J_{\Delta_{G}}+md^{2}$$
      where $d$ is the distance between the axes.
- **Moments of Inertia w.r.t. Planes and Points:**
    - **Plane XOY:** $J_{XOY}=\int_{S}z^{2}dm$
    - **Point O:** $J_{O}=\int_{S}OP^{2}dm=\int_{S}(x^{2}+y^{2}+z^{2})dm$
    - **Relation:** $J_{O}=\frac{1}{2}(J_{xx}+J_{yy}+J_{zz})$
- **Rules for Calculating $J(S)$ with Symmetries (at point A, in basis (X, Y, Z)):**
    - **Rule 1: Axis of Symmetry (A, Z):** $D=E=0$.
    - **Rule 2: Axis of Revolution (A, Z):** $A=B$.
    - **Rule 3: Plane of Symmetry (A, X, Y):** $D=E=0$.
    - **Rule 4: Two Axes of Symmetry ($\Delta_1, \Delta_2$):** The frame is a **principal inertia frame** (matrix is diagonal: $D=E=F=0$).
    - **Rule 5: Two Planes of Symmetry ($\Pi_1, \Pi_2$):** The frame is a **principal inertia frame** for any $Q$ at the intersection $\Pi_1 \cap \Pi_2$ (matrix is diagonal: $D=E=F=0$).

---
## 📝 Notes
- The center of mass $G$ and the inertia matrix $J(A, S)$ are **fundamental** for describing the solid's dynamics.
- The time parameter $t$ is initially ignored to study the solid's **intrinsic properties**.
- Knowledge of $G$ is crucial for calculating the **momentum** and **dynamic resultant**.
- The inertia operator $J(S)$ is necessary only if there is a **rotation** ($\omega_{S/R} \neq 0$).
- Material symmetries are used to **avoid complex integral calculations** by predicting the position of $G$ or the structure of $J(S)$.