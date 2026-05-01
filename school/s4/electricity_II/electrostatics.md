---
aliases:
  - Chapter_I
---
## 📚 Course Structure
- Section 1: **electrostatic force and field** 
- Section 2: **electrical potential**
- Section 3: **electrostatic depole**
- Section 4: **conductors**
- Section 5: **electrostatic energy**
 
---
## 📐 Equations & Concepts
#### electrostatic force and field:
- **electrostatic force:**
	- **Coulomb Law:**
		$$\vec{F}_{1,2} = \frac{1}{4\pi \epsilon_0} \frac{q_1q_2}{r} \vec{u}_{1,2}= -\vec{F}_{2,1}$$
	- **superposition:**
	the force done by multiple $q_i$ on a $q_0$ it's the sum of the forces.
- **electrostatic field:**
	- **Coulomb Law:**
		$$\vec{E}=\frac{\vec{F}}{q_0}$$
	the field created by multiple charges is the sum of the fields.
	$$\vec{E}0=\sum_i\vec{E}_i, \vec{E}=\int\vec{E}$$
	- **Gauss Theorem:**
	this only work for perfect symmetry cases
	the **flux** is given by : $$\Phi(\vec{E}/\sum) = \oint_\sum \vec{E}\vec{ds}= \frac{Q_{int}}{\epsilon_0}$$
	and in the local form is : $$Q_{int}=\iiint_v\rho dv$$ then $div \vec{E} = \frac{\rho}{\epsilon_0}$ which is the local Gauss local theorem. 
	Let $S$ be a charged surface with density $\sigma$. then we have :
	- the discontinuity of the normal component  of $\vec{E}$ $$(\vec{E}_1 \vec{n}_1 - \vec{E}_2 \vec{n}_1) = \frac{\sigma}{\epsilon_0}$$
	- the continuity of the tangant component of $\vec{E}$ $$\vec{E}_1 \vec{T} - \vec{E}_2 \vec{T} = 0$$
#### Electrical potential
Let there be a region in space where there's an electrical field $\vec{E}$. the circulation of $\vec{E}$ in $\Gamma$ between two points $A$ and $B$ is given by: $$C(\vec{E}/\Gamma) = \int_{Gamma} \vec{E} \vec{dl} = - \int_A^B dV = V_A - V_B$$
- **potential created by a singular point:**
	$V(M) = \frac{1}{4\pi \epsilon_0}\frac{q}{r}$
- **potential created by a distribution of charges:**
	- **discrete distribution**
		$V=\sum V_i$
	- **continuous distribution**
		$V=\frac{1}{4\pi \epsilon_0} \int \frac{dq}{r}$
- **equipotentials surface:**
	 $V=ctse \implies \vec{E}=-\vec{grad}V$
	- **Laplace and Poisson Equations**
		$\Delta V + \frac{\rho}{\epsilon_0} = 0$ (Poisson equation)
		where's there's no charge ($\rho = 0$)
		$\Delta V = 0$

#### Electrostatic Dipole
	$V(M)= \frac{\vec{p}.\vec{r}}{4\pi \epsilon_0 r^2} = \frac{\rho cos \theta}{4\pi\epsilon_0 r^2}$
	the field created is given by :$$\vec{E}(M) = \begin{cases}E_r = - \frac{\partial V}{\partial r} = \frac{\rho cos \theta}{4\pi \epsilon_0 r^3} \\ E_{\theta} = - \frac{1}{r}\frac{\partial V}{\partial \theta} = \frac{2\rho sin \theta}{4\pi \epsilon_0 r^3}\end{cases}$$

#### Conductors
- **equilibred conductors**
	- **proprieties**
		- $\vec{E}$ and $\rho$ are null inside the conductor.
		- the potential is constant inside it and in the surface.
		- the lines of the field are perpendiculars.
		- close to the conductor we have $E=\frac{\sigma}{\epsilon_0}$.
	- **Capacity**
		$C=\frac{Q}{V}$
- **Capacitors**
	- **Capacity**
		$dQ = CdV = C.d(V_A -V_B) \implies i = \frac{dQ}{dt}=C\frac{dV}{dt}$, $V = \frac{1}{C}\int i.dt$. 
	- **groups**
		- **series**
			$\frac{1}{C}=\sum_i \frac{1}{C_i}$
		- **parallel** 
			$C=\sum_i C_i$

#### Electrostatic Energy 
- **single charges**
	- **for a single charge**
		$W=qV(M)$
	- **for multiple charges**
		$W= \frac{1}{2}\sum_iq_i V_i$
- **case of conductors**
	- for a conductor with charge $Q$ and $V$ $$W = \frac{1}{2}QV$$
	- for a set of conductors $$W = \frac{1}{2} \sum_i Q_i V_i$$
- **Capacitors**
	$W=\frac{1}{2} QV = \frac{1}{2}CV^2 = \frac{1}{2}\frac{Q^2}{C}$
- **Location of electrostatic energy**
	$$\frac{dW}{dv} = \frac{1}{2} \epsilon_0 \vec{E^2}$$
---
## 📝 Notes
- $dq=\lambda dl$ in case of linear distribution $dq=\sigma ds$  in case of surface distribution, $dq=\rho dv$ in case of volumetric distribution.
- if the trajectory is closed the $\oint \vec{E} \vec{dl} = 0 \iff \vec{rot\vec{E}} = 0$.
- $\vec{E} = - \vec{grad} V$ and $\vec{E} = - \frac{dV}{dr}$.