---
aliases:
  - chapter_I
---
## 📚 Course Structure
- Section 1: **Spherical Diopters: Definitions & Properties**
- Section 2: **Stigmatism (Exact & Approximate)**
- Section 3: **Fundamental Invariant & Conjugation Formulas**
- Section 4: **Focal Points & Magnification**
- Section 5: **Image Construction & Special Rays**

---
## 📐 Equations & Concepts
#### Spherical Diopters: Definitions & Properties
- **Spherical Diopter:** Interface between two transparent, homogeneous, isotropic media (indices $n_1$, $n_2$) separated by a spherical surface (center $C$, summit $S$).
- **Principal Axis:** Line through $C$ and $S$.
- **Radius of Curvature:** $R = CS$.
- **Convergent/ Divergent:**
  - Convergent if $C$ is in the more refractive medium ($n_2 < n_1$).
  - Divergent if $C$ is in the less refractive medium ($n_2 > n_1$).

#### Stigmatism (Exact & Approximate)
- **Exact Stigmatism:** For some points, all rays from $A_1$ converge at $A_2$ after refraction.
- **Approximate Stigmatism (Gauss Conditions):** For rays close to the axis and small angles (paraxial), stigmatism is approximately achieved. Useful region is near $S$.

#### Fundamental Invariant & Conjugation Formulas
- **Fundamental Invariant:**
  - For a ray from $A$ to $A'$ through the diopter:
    $$
    n_1 \frac{\sin i_1}{CA_1} = n_2 \frac{\sin i_2}{CA_2}
    $$
  - In Gauss conditions (small angles):
    $$
    \frac{n_1}{CA_1} = \frac{n_2}{CA_2}
    $$
- **Conjugation Formula (Origin at Summit $S$):**
  $$
  \frac{n_2}{SA_2} - \frac{n_1}{SA_1} = \frac{n_2 - n_1}{SC}
  $$
- **Magnification (at $S$):**
  $$
  y = \frac{n_1 SA_2}{n_2 SA_1}
  $$
  - $y > 0$: image upright; $y < 0$: image inverted.
  - $|y| > 1$: image larger; $|y| < 1$: image smaller.

- **Conjugation Formula (Origin at Center $C$):**
  $$
  \frac{n_1}{CA_1} + \frac{n_2}{CA_2} = 0
  $$

#### Focal Points & Magnification
- **Focal Points:**
  - **Image Focal Point $F'$:** Where image forms when object is at infinity.
    $$
    f' = SF' = \frac{n_2 SC}{n_2 - n_1}
    $$
  - **Object Focal Point $F$:** Where object must be for image at infinity.
    $$
    f = SF = \frac{n_1 SC}{n_1 - n_2}
    $$
  - **Relation:** $f + f' = SC$
- **Vergence:**
  $$
  V = \frac{n_2 - n_1}{SC}
  $$

#### Image Construction & Special Rays
- **Special Rays for Construction:**
  - Ray through $C$ is undeviated.
  - Ray through object focal point $F$ emerges parallel to axis.
  - Ray parallel to axis passes through image focal point $F'$ after refraction.
- **Image Characteristics:**
  - Position: $SA'$
  - Nature: real if $SA' > 0$, virtual if $SA' < 0$
  - Orientation: upright if $y > 0$, inverted if $y < 0$
  - Size: $|y| > 1$ (enlarged), $|y| < 1$ (reduced), $y = 1$ (same size)

---
## 📝 Notes
- Spherical diopters relate object and image positions via conjugation formulas.
- Focal points and distances are key for ray tracing and image construction.
- Magnification tells you the size and orientation of the image.
- Use special rays for quick geometric constructions of images.
- The sign conventions (directions, indices) are crucial for correct results.
