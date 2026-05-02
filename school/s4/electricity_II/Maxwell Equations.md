---
aliases:
  - Chap_IV
---
# Maxwell equations in a static regime
- in electrostatics  : $\vec{j} = \vec{0}$
- in magneto-statics : $div \vec{j} = 0 = \frac{\partial \rho}{\partial t}$
	- $div \vec{E} = \frac{\rho}{\epsilon_0}$, $\Phi(\vec{E}) = \frac{\sum q_{int}}{\epsilon_0}$
	- $\vec{rot\vec{E}} = \vec{0}$, $\vec{E} = - \vec{grad} V$
	- $\vec{rot\vec{B}} = \mu_0 \vec{j}$, $\oint_C \vec{B}.d\vec{l} = \mu_0 \sum I_{int}$
	- $div\vec{B} = 0$, $\vec{B} = \vec{rot\vec{A}}$
- other relationships : 
	- when $v(\infty) = 0$ $$V= \frac{1}{4\pi  \epsilon_0} \iiint \frac{\rho d\tau}{r}$$
	- if $v$ is not infinite $$\vec{A} = \frac{\mu_0}{4\pi} \iiint \frac{\vec{j}d\tau}{r}$$
# Maxwell equation in function of time
## In the void
### Gauss Theorem 
- integral form : $$\iint \vec{E}(M,t) d\vec{S} = \frac{1}{\epsilon_0} \iiint_t \rho(M,t)d\tau$$
- Local form : $$div\vec{E}(M,t) = \frac{\rho (M,t)}{\epsilon_0}$$
### $\vec{B}$ is always a flux conservative
- $\Phi = \iint \vec{B}(M,t)d\vec{S} = 0$ 
- $div\vec{B}(M,t) = 0$

### Faraday law is always verified
- integral form : $\oint_c \vec{E}(M,t) d \vec{l} = - \frac{\partial}{\partial t} \iint_S \vec{B}(M,t)d\vec{S}$ 
- local form : $\vec{rot\vec{E(M,t)}} = - \frac{\partial \vec{B}(M,t)}{\partial t}$ and $\vec{E}(M,t) = - \vec{grad} V(M,t) - \frac{\partial \vec{A}(M,t)}{\partial t}$ 
### Ampere Theorem in variable regime
$$\vec{rot\vec{B}}(M,t) = \mu_0 (\vec{j}(M,t) + \epsilon_0 \frac{\partial \vec{E} (M,t)}{\partial t})$$
# passage relationships between two places
- $E_{1T} = E_{2T}$
- $\vec{D}_{2N} -  \vec{D}_{1N} = \sigma_{free}.\vec{n}$.
- $B_{1N} = B_{2N}$
- $\vec{H}_{1T} - \vec{H}_{2T} = \vec{J}_s \times \vec{n}$.