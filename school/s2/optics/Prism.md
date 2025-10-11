---
aliases:
  - chapter_III
---
## 📚 Course Structure
- Section 1: **Prism Basics & Dispersion**
- Section 2: **Fundamental Prism Relations**
- Section 3: **Deviation Angle & Its Calculation**
- Section 4: **Minimum Deviation & Refractive Index**
- Section 5: **Wavelength Dependence & Dispersion**

---
## 📐 Equations & Concepts
#### Prism Basics & Dispersion
- **Prism:** Transparent medium (index \( n \)) with two plane faces meeting at angle \( A \) (apex angle).
- **Dispersion:** When white light passes through a prism, it splits into its component colors (spectrum) due to wavelength-dependent refraction.
- **Visible Spectrum:** Wavelengths from 400 nm (violet) to 800 nm (red).
- **Application:** Used to analyze light from stars and identify chemical elements by their spectral lines.

#### Fundamental Prism Relations
- **Angles:**
  - \( i \): Angle of incidence (entry face)
  - \( r \): Angle of refraction (entry face)
  - \( r' \): Angle of incidence (exit face, inside prism)
  - \( i' \): Angle of emergence (exit face)
  - \( A \): Apex angle of the prism
- **Snell-Descartes Laws:**
  - At entry: \( \sin i = n \sin r \)
  - At exit: \( \sin i' = n \sin r' \)
- **Apex Relation:**
  - \( A = r + r' \)

#### Deviation Angle & Its Calculation
- **Deviation Angle (\( D \)):**
  - The angle between the incident and emergent rays.
  - \( D = i + i' - A \)
- **Expressing \( D \) as a function of \( i \):**
  - Use Snell's law and apex relation to relate all angles.
  - \( i' = \arcsin(n \sin r') = \arcsin(n \sin(A - r)) \)
  - \( r = \arcsin(\sin i / n) \)
  - Final formula:
    $$
    D = i + \arcsin\left(n \sin\left(A - \arcsin\left(\frac{\sin i}{n}\right)\right)\right) - A
    $$

#### Minimum Deviation & Refractive Index
- **Minimum Deviation (\( D_m \)):**
  - Occurs when \( i = i' \) and \( r = r' = A/2 \).
  - \( D_m = 2i - A \), so \( i = (A + D_m)/2 \).
  - \( r = A/2 \).
- **Refractive Index from Minimum Deviation:**
  - \( \sin i = n \sin r \Rightarrow n = \frac{\sin((A + D_m)/2)}{\sin(A/2)} \)

#### Wavelength Dependence & Dispersion
- **Cauchy's Law:**
  - \( n = a + \frac{b}{\lambda^2} \), where \( a, b \) are material constants, \( \lambda \) is wavelength.
  - As \( \lambda \) decreases (from red to violet), \( n \) increases, so deviation \( D \) increases.
  - Red light is less deviated than violet light.

---
## 📝 Notes
- A prism disperses light because its refractive index varies with wavelength.
- The deviation angle depends on the prism's apex angle, refractive index, and the angle of incidence.
- Minimum deviation is used to measure the refractive index of the prism material.
- The spectrum produced by a prism allows identification of chemical elements in light sources.
- For each incident angle, there are two conjugate planes (homocentric planes) related by the prism's geometry.
