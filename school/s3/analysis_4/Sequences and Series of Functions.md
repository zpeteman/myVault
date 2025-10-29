---
aliases:
  - Chapitre_II
---

## 📚 Course Structure
- Section 1: **Sequences of Functions**
- Section 2: **Series of Functions**

---

## 📐 Equations & Concepts

### Sequences of Functions

* **Definition: Simple Convergence (C.S)**
    A sequence of functions $(f_{n})_{n\in\mathbb{N}}$ converges simply (C.S) to a function $f$ on $I$ if and only if for all $x \in I$, $\lim_{n\rightarrow+\infty} f_{n}(x) = f(x)$.
    This means:
    $$\forall \epsilon > 0, \forall x \in I, \exists \eta(\epsilon, x) \in \mathbb{N} \text{ such that } n \ge \eta(\epsilon, x) \Rightarrow |f_{n}(x)-f(x)| \le \epsilon.$$

* **Definition: Uniform Convergence (C.U)**
    The sequence $(f_{n})_{n\in\mathbb{N}}$ converges **uniformly** (C.U) to $f$ on $I$ ($f_{n}\Rightarrow f$ on $I$) if and only if:
    $$\forall \epsilon > 0, \exists \eta(\epsilon) \in \mathbb{N} \text{ independent of } x \in I, \text{ such that } n \ge \eta(\epsilon) \Rightarrow \sup_{x\in I}|f_{n}(x)-f(x)| \le \epsilon.$$
    -   **Norm of Uniform Convergence:** The uniform norm on $I$ is defined as $||f|| = \sup_{x\in I} |f(x)|$.

* **Criterion of Continuity (Théorème 3.1.2)**
    If a sequence $(f_{n})_{n}$ converges **uniformly** to $f$ on $I$, and $f_{n}(x)$ is **continuous** at a point $x_{0}\in I$ for all $n$, then the limit function $f(x)$ is also continuous at $x_{0}$.
    -   **Note:** If the functions $f_{n}(x)$ are continuous on $I$ but the limit function $f(x)$ is not, then the convergence cannot be uniform.

* **Criterion of Integration (Théorème 3.1.3)**
    Let $(f_{n})_{n\in\mathbb{N}}$ be a sequence of continuous functions on a **compact interval** $I=[a,b]\subset\mathbb{R}$ such that $f_{n}\Rightarrow f$ on $I$. Then:
    1.  $f$ is integrable on $I$.
    2.  The limit can be moved inside the integral:
        $$\forall \alpha,\beta\in I, \lim_{n\rightarrow+\infty}\int_{\alpha}^{\beta}f_{n}(x)dx=\int_{\alpha}^{\beta}f(x)dx.$$

* **Criterion of Derivation (Théorème 3.1.4)**
    Let $(f_{n})_{n\in\mathbb{N}}$ be a sequence of functions of class $C^{1}$ on $I=[a,b]$ such that:
    1.  The sequence of derivatives $(f_{n}^{\prime})_{n\in\mathbb{N}}$ converges **uniformly** on $I$ towards a function $g$.
    2.  $\exists x_{0}\in I,$ such that $\lim_{n\rightarrow+\infty}f_{n}(x_{0})=l$ with $l$ finite.
    Then:
    -   $f_{n}$ converges **uniformly** on $I$ towards $f(x)=l+\int_{x_{0}}^{x}g(t)dt$.
    -   $f$ is of class $C^{1}$ on $I$ and $f^{\prime}=g$.

---

### Series of Functions

* **Definition: Normal Convergence**
    The series $\sum_{n}f_{n}(x)$ converges **normally** on $I$ if and only if the series of norms $\sum_{n}||f_{n}||$ converges.

* **Weierstrass Criterion (Théorème 3.2.4)**
    Let $(f_{n})_{n\in\mathbb{N}}$ be a sequence of functions on $I$ and $(v_{n})_{n}$ a convergent real numerical series ($\sum_{n}v_{n}$ converges). If a numerical majorant exists such that $\forall x\in I,\forall n\in\mathbb{N}$, $|f_{n}(x)|\le v_{n}$, then the series $\sum_{n}f_{n}(x)$ converges **normally**.

* **Relationship between Normal and Uniform Convergence (Théorème 3.2.5)**
    If the series $\sum_{n}f_{n}(x)$ converges **normally** on $I$, then it converges **uniformly** on $I$.

* **Criterion of Continuity (Théorème 3.2.8)**
    If $\sum_{n}f_{n}(x)$ is a series of functions that converges **uniformly** towards its sum $S$ on $I$, and $\forall n\in\mathbb{N}$, $f_{n}(x)$ is **continuous** at $x_{0}\in I$, then its sum $S(x)=\sum_{n=0}^{\infty}f_{n}(x)$ is continuous at $x_{0}$.

* **Criterion of Integration (Théorème 3.2.9)**
    If $\sum_{n}f_{n}(x)$ is a series of continuous functions that converges **uniformly** towards its sum $S$ on $I$, then:
    -   The integral and summation can be interchanged on a given interval $[\alpha,\beta]$:
        $$\sum_{n=0}^{\infty}\int_{\alpha}^{\beta}f_{n}(t)dt=\int_{\alpha}^{\beta}\sum_{n=0}^{\infty}f_{n}(t)dt=\int_{\alpha}^{\beta}S(t)dt.$$

* **Criterion of Derivation (Théorème 3.2.10)**
    Given a series of derivable functions $\sum_{n}f_{n}(x)$ where $f_{n}^{\prime}$ is defined and continuous on $I$. If:
    1.  The series of derivatives $\sum_{n}f_{n}^{\prime}(x)$ converges **uniformly** on every closed bounded interval of $I$.
    2.  $\exists x_{0}\in I$, such that the series $\sum_{n}f_{n}(x_{0})$ converges.
    Then the sum $S(x)=\sum_{n=0}^{\infty}f_{n}(x)$ is continuously differentiable on $I$ and:
    $$(\sum_{n=0}^{\infty}f_{n}(x))^{\prime}=\sum_{n=0}^{\infty}f_{n}^{\prime}(x).$$

* **Example Application: Sum of $\sum_{n\ge1}\frac{x^{n}}{n}$**
    For $x\in[-R,R]$ with $0<R<1$, the sum $S(x)$ is found using the derivation criterion:
    $$S^{\prime}(x)=\sum_{n=1}^{\infty}x^{n-1} = \frac{1}{1-x}.$$
    Integrating and using the fact that $S(0)=0$, the sum is:
    $$S(x) = \int_{0}^{x}\frac{1}{1-t}dt = -ln(1-x).$$

---

## 📝 Notes

* **Uniform vs. Simple Convergence:** Uniform convergence always implies simple convergence, but the converse is false.
* **Checking for Non-Uniform Convergence:** If $f_{n}$ are continuous on $I$ but the limit function $f$ is discontinuous on $I$, then the convergence is **not uniform**.
* **Weierstrass Criterion Note:** The normal convergence criterion is satisfied if the series of the uniform norms, $\sum_{n}||f_{n}||$, converges.
* **Compactness for Integration:** The compactness of the interval $I$ (i.e., being closed and bounded) is generally **necessary** for the Integration Criterion (Théorème 3.1.3). The interchange of limit and integral is not guaranteed over unbounded intervals, even with uniform convergence. For $I=[0,+\infty[$:
    $$\lim_{n\rightarrow+\infty}\int_{0}^{+\infty}f_{n}(x)dx=\frac{1}{6} \ne 0 = \int_{0}^{+\infty}\lim_{n\rightarrow+\infty}f_{n}(x)dx.$$