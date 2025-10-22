---
aliases:
  - Chapitre_II
---
## 📚 Course Structure

- Section 1: Sequences of Functions
- Section 2: Pointwise Convergence
- Section 3: Uniform Convergence
- Section 4: Fundamental Theorems

## 📐 Equations & Concepts

#### Sequences of Functions:
A sequence of functions on interval $I$ is an application $f: \mathbb{N} \to F(I, K)$ where $(f_n)_{n \in \mathbb{N}}$ maps $x \mapsto f_n(x)$

#### Pointwise Convergence:
$(f_n)_{n \in \mathbb{N}}$ converges pointwise to $f$ on $I$ if: $$\forall x \in I, \lim_{n \to +\infty} f_n(x) = f(x)$$$$\forall \epsilon > 0, \forall x \in I, \exists \eta(\epsilon, x) \in \mathbb{N} \text{ such that } n \geq \eta(\epsilon, x) \Rightarrow |f_n(x) - f(x)| \leq \epsilon$$

#### Uniform Convergence:
**Uniform Convergence Norm**: $$|f| = \sup_{x \in I} |f(x)|$$
$(f_n)_{n \in \mathbb{N}}$ converges uniformly to $f$ on $I$ (written $f_n \Rightarrow f$) if: $$\forall \epsilon > 0, \exists \eta(\epsilon) \in \mathbb{N} \text{ (independent of } x) \text{ such that } n \geq \eta(\epsilon) \Rightarrow |f_n - f| \leq \epsilon$$
**Equivalent form**: $$n \geq \eta(\epsilon) \Rightarrow \sup_{x \in I} |f_n(x) - f(x)| \leq \epsilon$$
#### Fundamental Theorems:
- **Cauchy Criterion:**
	$f_n$ converges uniformly to $f$ on $I$ if and only if: $$\forall \epsilon > 0, \exists \eta(\epsilon) \in \mathbb{N} \text{ such that } n \geq \eta(\epsilon), m \geq \eta(\epsilon) \Rightarrow |f_n - f_m| \leq \epsilon$$
- **Continuity Criterion:**
	If $(f_n)_n$ converges uniformly to $f$ on $I$ and each $f_n$ is continuous on $I$, then $f$ is continuous on $I$
- **Integration Criterion:**
	If $(f_n)_{n \in \mathbb{N}}$ is a sequence of continuous functions on $I = [a,b]$ such that $f_n \Rightarrow f$ on $I$, then:
	- $f$ is integrable on $I$
	- $\forall \alpha, \beta \in I$: $$\lim_{n \to +\infty} \int_{\alpha}^{\beta} f_n(x)dx = \int_{\alpha}^{\beta} f(x)dx$$
	- $\forall \alpha \in I$: $F_n(x) = \int_{\alpha}^{x} f_n(t)dt$ converges uniformly to $F(x) = \int_{\alpha}^{x} f(t)dt$
## 📝 Notes
- Uniform convergence is stronger than pointwise convergence - if $f_n$ converges uniformly to $f$, then it converges pointwise to $f$
- If all $f_n$ are continuous on $I$ but $f$ is not continuous on $I$, then $f_n$ does NOT converge uniformly to $f$ on $I$
- The compactness of interval $I$ is necessary for the integration theorem - without it, the result may not hold even if other conditions are satisfied
- For uniform convergence: $$\left|\int_{\alpha}^{\beta} f_n(x)dx - \int_{\alpha}^{\beta} f(x)dx\right| \leq (\beta - \alpha)|f_n - f|$$
- If $f_n \Rightarrow f$, then $F_n(x) = \int_{\alpha}^{x} f_n(t)dt$ also converges uniformly with bound $|F_n - F| \leq (b-a)|f_n - f|$