---
aliases:
  - Chapter_IV
---
## 📚 Course Structure
- Section 1: **piecewise continuity** 
- Section 2: **Fourier's coefficients**
- Section 3: **Fourier Series**
- Section 4: **Convergence of the Fourier Series**

---
## 📐 Equations & Concepts
#### piecewise continuity :
$f$ is piecewise continuous on $\mathbb{R}$ if it is piecewise continuous on every segment of $\mathbb{R}$.

#### Fourier's coefficients :  
- **Complex Coefficients :** 
	Let  be a -periodic and piecewise continuous function on $\mathbb{R}$.  
	The **exponential Fourier coefficients** of  are the complex numbers defined by: $$
c_n = \frac{1}{T} \int_0^T e^{-in\omega t} f(t) \, dt,
\qquad n \in \mathbb{Z}, \quad \omega = \frac{2\pi}{T}.
$$
- **real(Trig) Coefficients :** 
	The **trigonometric Fourier coefficients** are defined as follows: $$
a_0 = \frac{2}{T} \int_0^T f(t) \, dt 
     = \frac{2}{T} \int_\alpha^{T+\alpha} f(t) \, dt,
     \qquad \alpha \in \mathbb{R}.
$$
	For $n \in \mathbb{N}^*$ and $\alpha \in \mathbb{R}$: $$
a_n = \frac{2}{T} \int_0^T f(t)\cos(n\omega t) \, dt
     = \frac{2}{T} \int_\alpha^{T+\alpha} f(t)\cos(n\omega t) \, dt,
$$  $$
b_n = \frac{2}{T} \int_0^T f(t)\sin(n\omega t) \, dt
     = \frac{2}{T} \int_\alpha^{T+\alpha} f(t)\sin(n\omega t) \, dt.
$$

#### Fourier Series
The Fourier series of  is defined by: $$
\frac{a_0}{2} + \sum_{n \ge 1} \left[ a_n \cos(n\omega t) + b_n \sin(n\omega t) \right]
$$
It can also be expressed using the **exponential coefficients**: $$
\sum_{n \in \mathbb{Z}} c_n e^{in\omega t}
$$
#### Convergence of the Fourier Series
-  **Dirichlet’s Theorem :**
	Let $f$ be a $T$-periodic function, piecewise continuous and piecewise of class $C^1$ on $\mathbb{R}$.  Then, the Fourier series of $f$ converges **pointwise** to the function: $$
\tilde{f}(x) = \frac{f(x + 0) + f(x - 0)}{2}, \qquad \forall x \in \mathbb{R}
$$
	where $f(x + 0)$ and $f(x - 0)$ are the **right-hand** and **left-hand limits** of $f$ at $x$ respectively. If $f$ is continuous, the convergence is **uniform**.

---
## 📝 Notes
- $f$ and $g$ are both piecewise continuous then $f+g$ is piecewise continuous and $\lambda f$ is piecewise continuous too. 
- $f$ is piecewise continuous in a segment that means it does have a limit and derivative in that segment.
- $c_n$ are the **complex (exponential)** Fourier coefficients.  
- $a_n$ and $b_n$ are the **real (trigonometric)** Fourier coefficients. 
- They express a $T$-periodic function as a sum of sines, cosines, or complex exponentials.
- At points of discontinuity, Fourier series converges to the average of the right and left limits.  
- f $f$ is continuous, convergence Fourier series becomes uniform.