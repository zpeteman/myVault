---
aliases:
  - chapter_0
---
## 📚 Course Structure
- Section 1: **Vectors & Coordinate Systems**
- Section 2: **Vector Operations (Dot & Cross Product)**
- Section 3: **Coordinate Systems (Cartesian, Cylindrical, Spherical)**
- Section 4: **Vector Analysis (Gradient, Divergence, Curl, Laplacian)**
- Section 5: **Vector Integrals (Circulation, Flux, Stokes & Green's Theorems)**
- Section 6: **Solid Angle**

---
## 📐 Equations & Concepts
#### Vectors & Coordinate Systems
- **Vector Definition:** Oriented quantity with direction and magnitude (e.g., velocity, gravitational field).
- **Notation:** A vector from $A$ to $B$ is $\overrightarrow{AB}$; its magnitude is $|\overrightarrow{AB}|$.
- **Unit Vector:** $\vec{u} = \frac{\vec{V}}{|\vec{V}|}$
- **Components:** In basis $\vec{i}, \vec{j}, \vec{k}$, $\vec{V} = x\vec{i} + y\vec{j} + z\vec{k}$, $|\vec{V}| = \sqrt{x^2 + y^2 + z^2}$

#### Vector Operations (Dot & Cross Product)
- **Dot Product:** $\vec{V}_1 \cdot \vec{V}_2 = |\vec{V}_1||\vec{V}_2|\cos\theta$
  - Properties: Zero if vectors are orthogonal; commutative; distributive.
  - In components: $\vec{V}_1 \cdot \vec{V}_2 = x_1x_2 + y_1y_2 + z_1z_2$
- **Cross Product:** $\vec{V}_1 \times \vec{V}_2$ is a vector perpendicular to both, with magnitude $|\vec{V}_1||\vec{V}_2|\sin\theta$
  - Properties: Zero if vectors are parallel; anti-commutative; distributive.
  - In components:
    $$
    \vec{V}_1 \times \vec{V}_2 = (y_1z_2 - z_1y_2)\vec{i} + (z_1x_2 - x_1z_2)\vec{j} + (x_1y_2 - y_1x_2)\vec{k}
    $$

#### Coordinate Systems
- **Cartesian:** $M(x, y, z)$, $\vec{OM} = x\vec{i} + y\vec{j} + z\vec{k}$
  - Elemental displacement: $d\vec{l} = dx\vec{i} + dy\vec{j} + dz\vec{k}$
  - Surface elements: $dxdy$ (in $\vec{i},\vec{j}$), $dxdz$ (in $\vec{i},\vec{k}$), $dydz$ (in $\vec{j},\vec{k}$)
  - Volume element: $dvdxdy dz$
- **Cylindrical:** $M(\rho, \varphi, z)$, $\vec{OM} = \rho\vec{e}_\rho + z\vec{e}_z$
  - $x = \rho\cos\varphi$, $y = \rho\sin\varphi$, $z = z$
  - Elemental displacement: $d\vec{l} = d\rho\vec{e}_\rho + \rho d\varphi\vec{e}_\varphi + dz\vec{e}_z$
  - Surface elements: $\rho d\varphi dz$, $d\rho dz$, $\rho d\rho d\varphi$
  - Volume element: $\rho d\rho d\varphi dz$
- **Spherical:** $M(r, \theta, \varphi)$, $\vec{OM} = r\vec{e}_r$
  - $x = r\sin\theta\cos\varphi$, $y = r\sin\theta\sin\varphi$, $z = r\cos\theta$
  - Elemental displacement: $d\vec{l} = dr\vec{e}_r + r d\theta\vec{e}_\theta + r\sin\theta d\varphi\vec{e}_\varphi$
  - Surface elements: $r^2\sin\theta d\theta d\varphi$, $r\sin\theta dr d\varphi$, $r dr d\theta$
  - Volume element: $r^2\sin\theta dr d\theta d\varphi$

#### Vector Analysis (Gradient, Divergence, Curl, Laplacian)
- **Gradient:** For scalar $f(x, y, z)$:
  $$
  \nabla f = \frac{\partial f}{\partial x}\vec{i} + \frac{\partial f}{\partial y}\vec{j} + \frac{\partial f}{\partial z}\vec{k}
  $$
- **Divergence:** For vector $\vec{V}(x, y, z)$:
  $$
  \nabla \cdot \vec{V} = \frac{\partial V_x}{\partial x} + \frac{\partial V_y}{\partial y} + \frac{\partial V_z}{\partial z}
  $$
- **Curl (Rotationnel):**
  $$
  \nabla \times \vec{V} = \left(\frac{\partial V_z}{\partial y} - \frac{\partial V_y}{\partial z}\right)\vec{i} + \left(\frac{\partial V_x}{\partial z} - \frac{\partial V_z}{\partial x}\right)\vec{j} + \left(\frac{\partial V_y}{\partial x} - \frac{\partial V_x}{\partial y}\right)\vec{k}
  $$
- **Laplacian:** For scalar $f$:
  $$
  \Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}
  $$

#### Vector Integrals (Circulation, Flux, Stokes & Green's Theorems)
- **Circulation:** Integral of $\vec{V}$ along curve $C$ from $A$ to $B$:
  $$
  \int_A^B \vec{V} \cdot d\vec{l}
  $$
  - If $\vec{V} = \nabla U$, circulation depends only on endpoints: $U(B) - U(A)$
  - On a closed path, circulation is zero if $\vec{V}$ is a gradient field.
- **Flux:** Through surface $S$ with normal $\vec{n}$:
  $$
  \int_S \vec{V} \cdot \vec{n} dS
  $$
- **Stokes' Theorem:**
  $$
  \int_C \vec{V} \cdot d\vec{l} = \int_S (\nabla \times \vec{V}) \cdot \vec{n} dS
  $$
  - Circulation around $C$ equals flux of curl through $S$.
  - If $\vec{V}$ is a gradient field, $\nabla \times \vec{V} = 0$.
- **Green-Ostrogradsky Theorem:**
  $$
  \int_S \vec{V} \cdot \vec{n} dS = \int_V (\nabla \cdot \vec{V}) dv
  $$
  - Flux through closed surface equals integral of divergence over volume.
  - If $\nabla \cdot \vec{V} = 0$, flux is zero (conservative field).

#### Solid Angle
- **Plane Angle:** $d\theta = \frac{dP}{R}$, $dP$ is arc length, $R$ is radius (unit: radian).
- **Solid Angle:** $d\Omega = \frac{dS}{R^2}$, $dS$ is surface area, $R$ is distance (unit: steradian).
  - For surface $S$ seen from $O$:
    $$
    \Omega = \int_S \frac{\vec{OM} \cdot \vec{n}}{|\vec{OM}|^3} dS
    $$

---
## 📝 Notes
- Vectors have direction and magnitude; their components depend on the chosen basis.
- Dot product gives a scalar; cross product gives a vector perpendicular to both inputs.
- Coordinate systems (Cartesian, cylindrical, spherical) are chosen based on symmetry.
- Gradient, divergence, curl, and Laplacian are key differential operators in vector analysis.
- Stokes' and Green's theorems relate integrals over curves, surfaces, and volumes.
- Solid angle generalizes plane angle to three dimensions; useful for flux calculations.
