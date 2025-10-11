---
aliases:
  - chapter_V
---
## 📚 Course Structure
- Section 1: **Centered Optical Systems: Definitions & Types**
- Section 2: **Lagrange-Helmholtz Invariant & Magnifications**
- Section 3: **Cardinal Points: Foci, Principal Points, Nodal Points**
- Section 4: **Conjugation, Focal Planes, and Image Construction**
- Section 5: **Vergence, Association of Systems, and Gullstrand's Formula**

---
## 📐 Equations & Concepts
#### Centered Optical Systems: Definitions & Types
- **Centered System:** Set of transparent media separated by plane or spherical surfaces sharing a common principal axis.
  - **Dioptric System:** Only diopters (refracting surfaces).
  - **Catadioptric System:** Both mirrors and diopters.
- **Examples:**
  - Lens: two spherical diopters
  - Ball: one plane, one spherical diopter
  - Ocular: two lenses
  - Silvered ball: plane diopter + concave spherical mirror

#### Lagrange-Helmholtz Invariant & Magnifications
- **Transverse Magnification:**
  $$
  G = \frac{A'B'}{AB}
  $$
- **Angular Magnification:**
  $$
  G_\alpha = \frac{\alpha'}{\alpha}
  $$
- **Lagrange-Helmholtz Invariant:**
  - For each component, and for the whole system:
    $$
    n_1 A_1B_1 \cdot \theta_1 = n_2 A_2B_2 \cdot \theta_2
    $$
  - In Gauss approximation (small angles):
    $$
    n_1 SA_2 = n_2 SA_1
    $$
    $$
    n_1 A_1B_1 \cdot \theta_1 = n_2 A_2B_2 \cdot \theta_2
    $$

#### Cardinal Points: Foci, Principal Points, Nodal Points
- **Foci:**
  - **Object Focus \( F \):** Point whose image is at infinity (emergent rays parallel to axis).
  - **Image Focus \( F' \):** Image of a point at infinity (incident rays parallel to axis).
  - **Focal Planes:** Perpendicular to axis through \( F \) or \( F' \).
- **Principal Points \( H, H' \):**
  - Intersection of principal planes with axis.
  - In Gauss approximation, often coincide with the summit \( S \) for a single diopter.
- **Nodal Points \( N, N' \):**
  - Points where an incident ray through \( N \) emerges parallel through \( N' \).
  - For identical external media, principal and nodal points coincide.
- **Optical Center \( O \):**
  - Point such that any ray through \( O \) is undeviated (for identical external media).

#### Conjugation, Focal Planes, and Image Construction
- **Conjugation Formula (Centered System):**
  - With origins at principal points \( H \) and \( H' \):
    $$
    \frac{HF}{HA} + \frac{H'F'}{H'A'} = 1
    $$
  - \( f = HF \), \( f' = H'F' \) are object and image focal distances.
- **Magnification:**
  $$
  \gamma = \frac{A'B'}{AB} = \frac{f'}{f}
  $$
- **Vergence:**
  $$
  V = \frac{n'}{f'} - \frac{n}{f}
  $$
  - In diopters (m\(^{-1}\)). \( V > 0 \): convergent, \( V < 0 \): divergent.
- **Image Construction:**
  - Use principal rays and similar triangles.
  - For each system, image construction proceeds stepwise through each component.

#### Association of Centered Systems & Gullstrand's Formula
- **Association:**
  - Two centered systems \( S_1 \) and \( S_2 \) with axes aligned can be combined into an equivalent system \( S \).
  - The cardinal points and focal distances of \( S \) are determined from those of \( S_1 \) and \( S_2 \) and their separation \( e \).
- **Gullstrand's Formula:**
  - For two systems separated by \( e \) in medium of index \( N \):
    $$
    V = V_1 + V_2 - \frac{e V_1 V_2}{N}
    $$
  - \( V_1, V_2 \) are vergences of \( S_1, S_2 \).

---
## 📝 Notes
- Centered systems generalize single lenses/diopters to combinations, with shared principal axis.
- The Lagrange-Helmholtz invariant links object and image sizes, angles, and refractive indices.
- Cardinal points (foci, principal, nodal) are essential for describing image formation and system properties.
- The conjugation formula relates object and image positions via focal distances.
- Vergence describes the converging/diverging power of the system; Gullstrand's formula gives the total vergence for combined systems.
- For construction, always use the cardinal points and principal planes for reference.
