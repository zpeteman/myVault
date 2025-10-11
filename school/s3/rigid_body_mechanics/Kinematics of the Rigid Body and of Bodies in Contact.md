---
aliases:
  - Chap_II
---
## 📚 Course Structure
- Section 1: **Kinematics of the Rigid Body**
- Section 2: **Kinematics of Bodies in Contact**

---
## 📐 Equations & Concepts
#### Kinematics of the Rigid Body:
- **Definition:**
	A **rigid body** (S) is a set of material points, moving in time, that fulfils two properties: 
	- Indeformability (Rigidity) For any two points A, P of the solid: $$ \| \overrightarrow{AP} \| = \text{constant} \qquad \text{for all time t} $$ This means the distance between any two points of the solid remains unchanged over time (the solid is undeformable). 
	- Impenetrability For all $S_1, S_2 \subset S$, if $S_1 \cap S_2 = \varnothing$ at all times, then no part of the solid can penetrate any other part of the solid.
- **Degrees of Freedom (DoF) of a Rigid Body:**
	A rigid body S is studied relative to a fixed reference frame $R_0(O, \vec{x}_0, \vec{y}_0, \vec{z}_0)$. We often attach a moving frame $R_S(O_1, \vec{x}_1, \vec{y}_1, \vec{z}_1)$ to S, which moves in the same way as S (so all points in S are at rest in $R_S$).
	- **Six Parameters Are Required:** 
		To track the movement of $R_S$ relative to $R_0$, six parameters must be specified: 
		- The three coordinates $(x, y, z)$ of a chosen point (usually the centroid or centre of mass $G$) of S in $R_0$. 
		- The three Euler angles $\theta_1, \theta_2, \theta_3$ that describe the orientation of S.
		$\rightarrow$ In the most general case, a rigid body in space has **six degrees of freedom**.
	- **Degrees of Freedom (DoF):**
		The **degree of freedom** (n. d. d.) of a rigid body is the **number of independent parameters needed to completely describe its motion**k.	
- **Velocity Field of a Rigid Body:**
	For any two points $A$ and $P$ in a rigid body $S$, the distance $|\overrightarrow{AP}|$ remains constant over time.
	- **Time Derivative and Equiprojecitivity:**
		Taking the time derivative: $$ \frac{d}{dt} \left(|\overrightarrow{AP}|^2\right) = 2\,\overrightarrow{AP} \cdot \frac{d}{dt}(\overrightarrow{AP}) = 0 $$ So: $$ \overrightarrow{AP} \cdot [\vec{V}(P/R_0) - \vec{V}(A/R_0)] = 0 $$ Where $\vec{V}(P/R_0)$ and $\vec{V}(A/R_0)$ are the velocities of $P$ and $A$ relative to the fixed frame $R_0$. It follows that: $$ \overrightarrow{AP} \cdot \vec{V}(P/R_0) = \overrightarrow{AP} \cdot \vec{V}(A/R_0) $$
	- **Fundamental Relation for the Velocity Field:**
		There exists a unique vector $\vec{\Omega}(S/R_0)$ such that $$ \vec{V}(P/S/R_0) = \vec{V}(A/S/R_0) + \vec{\Omega}(S/R_0) \wedge \overrightarrow{AP} $$ This is the **fundamental relation for the velocity field of a rigid body**. 
		- $\vec{\Omega}(S/R_0)$ is called the **instantaneous angular velocity vector** relative to $R_0$. 
		- The velocity field is fully determined if the velocity of a single point AND the angular velocity are known with respect to the fixed frame.
	- **Velocity Wrench:**
		The velocity field of a rigid body can also be represented as the **velocity wrench**: $$ [T_{V}]_A = \left[\vec{\Omega}(S/R_0),\ \vec{V}(A/S/R_0)\right] $$ where $[T_{V}]_A$ is the velocity wrench at point $A$. 
		- $\vec{\Omega}(S/R_0)$ is the resultant (angular velocity) 
		- $\vec{V}(A/S/R_0)$ is the moment (velocity at $A$)
- **Acceleration Field of a Rigid Body:**
	Starting from the velocity field relation: $$ \vec{V}(P/S/R_0) = \vec{V}(A/S/R_0) + \vec{\Omega}(S/R_0) \wedge \overrightarrow{AP} $$ The acceleration of point $P$ of the solid is obtained by differentiating: $$ \dot{\vec{V}}(P/R_0) = \left[ \frac{d}{dt}\vec{V}(P/R_0) \right]_{R_0} $$ So: $$ \vec{\Gamma}(P/R_0) = \left[ \frac{d}{dt}\vec{V}(A/R_0) \right]_{R_0} + \left[ \frac{d}{dt}\vec{\Omega}(S/R_0) \right]_{R_0} \wedge \overrightarrow{AP} + \vec{\Omega}(S/R_0) \wedge \left( \vec{\Omega}(S/R_0) \wedge \overrightarrow{AP} \right) + \vec{\Omega}(S/R_0) \wedge \vec{V}(A/R_0) $$ The acceleration field for a rigid body is **not** antisymmetric and does **not** define a wrench.
- **Special Motions of a Rigid Body:**
	- **Pure Translation:**
		All points share the same velocity: $$ \vec{V}(P/R_0) = \vec{V}(A/R_0) $$ 
		The motion is **rectilinear** if $\vec{V}(A/R_0)$ is constant in magnitude and direction.
	- **Pure Rotation about a Fixed Axis:**
		If $\vec{V}(A/R_0) = \vec{0}$: $$ \vec{V}(P/R_0) = \vec{\Omega}(S/R_0) \wedge \overrightarrow{AP} $$ where $\vec{\Omega}(S/R_0)$ is the instantaneous angular velocity vector. 
		Scalar invariant: $$ \vec{\Omega}(S/R_0) \cdot \vec{V}(P/R_0) = 0 $$
	- **Helical Motion about an Axis through A:**
		Point $P$ undergoes both rotation about, and translation along, the axis $(O, \vec{z}_0)$: $$ \vec{V}(P/R_0) = \vec{V}(A/R_0) + \vec{\Omega}(S/R_0) \wedge \overrightarrow{AP} $$ This motion is a decomposition into a couple (rotation) and a collinear glisser (translation).
- **Composition of Instantaneous Rotation Vectors:**
	Let $A$ and $B$ be two points of the moving reference frame $R_1$.
	The instantaneous angular velocity of $R_2$ with respect to $R_0$ satisfies: $$ \vec{\Omega}(R_2/R_0) = \vec{\Omega}(R_2/R_1) + \vec{\Omega}(R_1/R_0) $$
	This generalizes for $N$ nested frames: $$ \vec{\Omega}(R_N/R_0) = \vec{\Omega}(R_N/R_{N-1}) + \vec{\Omega}(R_{N-1}/R_{N-2}) + \cdots + \vec{\Omega}(R_1/R_0) $$
	This rule allows for the sum of angular velocities across successive reference frame changes.
- **Euler Angles and Decomposition of Angular Velocity:**
	Euler angles $(\varphi,\, \theta,\, \psi)$ describe the orientation of a rigid body as a series of three elemental rotations: 
	1. **Precession**: By $\psi$ about the fixed axis $\vec{z}_0$ 
	2. **Nutation**: By $\theta$ about the intermediate axis $\vec{u}$ 
	3. **Proper Rotation**: By $\varphi$ about the body-fixed axis $\vec{z}$
	The corresponding instantaneous angular velocity for each is: 
	- Precession: $\vec{\Omega}(R_1/R_0) = \frac{d\psi}{dt} \vec{z}_0 = \dot{\psi}\, \vec{z}_0$ 
	- Nutation: $\vec{\Omega}(R_2/R_1) = \frac{d\theta}{dt} \vec{u} = \dot{\theta}\, \vec{u}$ 
	- Proper rotation: $\vec{\Omega}(R_3/R_2) = \frac{d\varphi}{dt} \vec{z} = \dot{\varphi}\, \vec{z}$
	The **total instantaneous angular velocity** of the solid with respect to the fixed frame is: $$ \vec{\Omega}(S/R_0) = \dot{\psi}\, \vec{z}_0 + \dot{\theta}\, \vec{u} + \dot{\varphi}\, \vec{z} $$
	This formula sums the rates of the three consecutive Euler rotations (expressed on the corresponding axes).
	

#### Kinematics of Bodies in Contact:
- **Point Contact Between Solids:**
	- **Definition:**
		Two solids $S_1$ and $S_2$ in motion in a reference frame $R_0(O, \vec{x}_0,\vec{y}_0,\vec{z}_0)$ are said to be in point contact if, at each instant, their surfaces touch and are tangent at a single point $I$, called the geometric contact point.
	- **Remark:**
		At the point of contact, distinguish between three coincident points: 
		- **Geometric contact point** $I$: at time $t$, $S_1 \cap S_2 = I$. 
		- **Material point $I_1$ of $S_1$:** coincides with $I$ at the instant. 
		- **Material point $I_2$ of $S_2$:** also coincides with $I$ at the instant. 
		These points $I$, $I_1$, and $I_2$ are identical at a given instant but usually have different trajectories and (initially) different velocities.
- **Sliding, Rolling, and Pivoting at a Contact Point:**
	- **Sliding Velocity:**
		The sliding velocity of solid $S_1$ on $S_2$ at instant $t$, at the contact point $I$, is: $$ \vec{V}_g(S_1/S_2) = \vec{V}(I/S_1) - \vec{V}(I/S_2) $$ Or with respect to a fixed reference $R_0$: $$ \vec{V}_g(S_1/S_2) = \vec{V}(I\in S_1/R_0) - \vec{V}(I\in S_2/R_0) $$ 
		- $\vec{V}_g(S_1/S_2)$ is contained in the tangent plane at the contact.
	- **Decomposition of Instantaneous Rotation:**
		The instantaneous angular velocity of $S_1$ relative to $S_2$ at the contact decomposes into: $$ \vec{\Omega}(S_1/S_2) = \vec{\Omega}_t(S_1/S_2) + \vec{\Omega}_n(S_1/S_2) $$ Where: 
		- $\vec{\Omega}_t$ is the instantaneous rolling angular velocity (tangent to the contact plane), 
		- $\vec{\Omega}_n$ is the instantaneous pivoting angular velocity (normal to the contact plane).
	- **Special Cases:**
		- **Rolling without slipping**: $\vec{V}_g(S_1/S_2) = \vec{0}$ 
		- **Pure pivoting**: $\vec{\Omega}_t = \vec{0}$



---
## 📝 Notes
- Velocity field: $\vec{V}(P) = \vec{V}(A) + \vec{\Omega} \wedge \overrightarrow{AP}$ 
- The acceleration field is not antisymmetric and does not form a wrench. 
- 6 parameters (3 positions, 3 orientations) fully define a rigid body's motion. 
- Total instantaneous angular velocity: $\vec{\Omega}_{\text{total}} = \sum \vec{\Omega}_{\text{partial}}$ 
- Euler angles can parameterize any 3D rotation. 
- Sliding velocity at contact: $\vec{V}_g(S_1/S_2) = \vec{V}(I/S_1) - \vec{V}(I/S_2)$, always tangent at contact. 
- No sliding $(\vec{V}_g = 0)$ means rolling without slip at that point. 
- Rolling and pivoting decompose angular velocity at contact. 
- The material, geometric, and coincident points at contact are only the same at an instant. 
- In translation, all points have equal velocities. 
- Pure rotation about axis through $A$: $\vec{V}(P/R_0) = \vec{\Omega} \wedge \overrightarrow{AP}$