---
aliases:
  - Chap_I
---
## 📚 Course Structure
- Section 1: **Review**
- Section 2: **Vectorial Division**
- Section 3: **Vector Fields**
- Section 4: **Wrenches**
---
## 📐 Equations & Concepts
#### Review:
$$
\begin{align*}
% Dot Product
\vec{U} \cdot \vec{V} 
    &= ||\vec{U}||\,||\vec{V}||\,\cos\theta = u_1 v_1 + u_2 v_2 + u_3 v_3 
    && \text{\quad [Dot Product]} \\[1.2em]
% Cross Product
\vec{U} \wedge \vec{V}
    &= 
    \begin{pmatrix} u_1 \\ u_2 \\ u_3 \end{pmatrix}
    \wedge
    \begin{pmatrix} v_1 \\ v_2 \\ v_3 \end{pmatrix}
    =
    \begin{pmatrix}
        u_2 v_3 - u_3 v_2 \\
        u_3 v_1 - u_1 v_3 \\
        u_1 v_2 - u_2 v_1
    \end{pmatrix}
    && \text{\quad [Cross Product]} \\[1.2em]
% Scalar Triple Product
\vec{U} \cdot (\vec{V} \wedge \vec{W}) 
    &= \vec{V} \cdot (\vec{W} \wedge \vec{U}) = \vec{W} \cdot (\vec{U} \wedge \vec{V})
    && \text{\quad [Scalar Triple Product]} \\[1.2em]
% Vector Triple Product
\vec{U} \wedge (\vec{V} \wedge \vec{W}) 
    &= (\vec{U} \cdot \vec{W}) \vec{V} - (\vec{U} \cdot \vec{V}) \vec{W} 
    && \text{\quad [Vector Triple Product]} \\[1.2em]
% Lagrange's Identity
(\vec{U} \wedge \vec{V}) \cdot (\vec{W} \wedge \vec{X}) 
    &= (\vec{U} \cdot \vec{W})(\vec{V} \cdot \vec{X}) - (\vec{U} \cdot \vec{X})(\vec{V} \cdot \vec{W})
    && \text{\quad [Lagrange's Identity]}
\end{align*}

$$

#### Vectorial Division:
Let $\vec{U}$ and $\vec{V}$ two non empty vectors in the victor field $E$. there's a vector $\vec{X}$ such that $$\vec{U}\wedge\vec{X} = \vec{V}$$
Given nonzero vectors $\vec{U}$ and $\vec{V}$ in a vector space, if $\vec{U} \cdot \vec{V} = 0$ (i.e., they are orthogonal), then the vector division of $\vec{V}$ by $\vec{U}$ yields:

$$
\vec{X} = -\frac{\vec{U} \wedge \vec{V}}{||\vec{U}||^2} + \alpha \vec{U}
$$

where $\alpha$ is a real parameter.

#### Vector Fields
- **Definition:**
	A vector field $\vec{U}$ is a function that assigns to each point $P$ in an affine 3D space $\xi_3$ a vector $\vec{U}(P)$ in a 3-dimensional vector space $E_3$: $$ \vec{U}: \begin{cases} \xi_3 \to E_3 \\ P \mapsto \vec{U}(P) \end{cases} $$ - $\xi_3$ is the space of points. - $E_3$ is the associated 3D vector space (the space of free vectors).
	- **Uniform Vector Field:**
		A vector field is **uniform** if: $$ \vec{U}(P) = \vec{U}(P_0) $$ for every point $P$.
	- **Affine Vector Field:**
		A vector field is **affine** if there exists a point $O$ and a linear map $\mathcal{E}$ such that: $$ \vec{U}(P) = \vec{U}(O) + \mathcal{E}(\overrightarrow{OP}) $$
	- **Linearity Of $\mathcal{E}$:**
		The map $\mathcal{E}$ is linear if and only if, for all real numbers $a, b$ and for all $\vec{u}, \vec{v}$ in $E_3$: $$ \mathcal{E}(a\vec{u} + b\vec{v}) = a\,\mathcal{E}(\vec{u}) + b\,\mathcal{E}(\vec{v}) $$
- **Antisymmetric and Equiprojective Vector Fields:**
	- **Antisymmetric:**
		A linear map $\mathcal{E}$ is antisymmetric in $E_3$ if: $$ \vec{u} \cdot \mathcal{E}(\vec{v}) + \vec{v} \cdot \mathcal{E}(\vec{u}) = 0 $$ or equivalently: $$ \vec{u} \cdot \mathcal{E}(\vec{v}) = -\vec{v} \cdot \mathcal{E}(\vec{u}) $$ A vector field is **antisymmetric** $\iff$ its associated linear application $\mathcal{E}$ is antisymmetric.
	- **Equiprojective:**
		A vector field $\vec{U}$ is **equiprojective** if: $$ \overrightarrow{PQ} \cdot \vec{U}(P) = \overrightarrow{PQ} \cdot \vec{U}(Q) $$ for all points $P, Q$.
- **Antisymmetric Vector Fields in $\mathbb{R}^3$:**
	In three dimensions, every antisymmetric or equiprojective vector field $\vec{U}$ corresponds to a unique vector $\vec{R}$, called the vector of the antisymmetric field. For any pair of points $(P, Q)$: $$ \vec{U}(Q) = \vec{U}(P) + \vec{R} \wedge \overrightarrow{PQ} $$ This is the fundamental relation for antisymmetric vector fields. The associated linear map $\mathcal{E}$ is given by: $$ \mathcal{E}(\vec{V}) = \vec{R} \wedge \vec{V} $$ for all $\vec{V}$ in the vector space.

#### Wrenches
- **Definition:**
	A **Wrench** $[T]$ is the set made up of an antisymmetric vector field $\vec{M}$ and its vector $\vec{R}$. At point $P$: $$ [T]_P = [\vec{R}, \vec{M}(P)] $$
	- $\vec{R}$: **general resultant** of the Wrench. 
	- $\vec{M}(P)$: **moment** of the Wrench at point $P$. Knowing $\vec{R}$ and $\vec{M}(A)$ at any point $A$ determines the field at any other point $P$: $$ \vec{M}(P) = \vec{M}(A) + \vec{R} \wedge \overrightarrow{AP} $$ This relation is **fundamental for the moment field of a Wrench**.
- **Components of a Wrenches:**
	In the direct orthonormal frame $R(O, \vec{i}, \vec{j}, \vec{k})$, the vectors $\vec{R}$ and $\vec{M}(O)$ are the six components of the torsor $[T]_O = [\vec{R}, \vec{M}(O)]$. In this order: $$ \vec{R} = \begin{pmatrix} X \\ Y \\ Z \end{pmatrix} \qquad \vec{M}(O) = \begin{pmatrix} L \\ M \\ N \end{pmatrix} $$
- **Equiprojectivity and Scalar Invariant of a Wrench:**
	The moment field of a wrench is equiprojective. For any points $P$ and $Q$: $$ \vec{M}(P) = \vec{M}(Q) + \vec{R} \wedge \overrightarrow{QP} $$ and equivalently: $$ \overrightarrow{QP} \cdot \vec{M}(P) = \overrightarrow{QP} \cdot \vec{M}(Q) $$ The scalar product $$ I = \vec{R} \cdot \vec{M}(P) $$ is called the **scalar invariant** of the wrench and does not depend on the chosen point $P$.
- **Vectorial Invariant of a Wrench:**
	Given a wrench $[W]_P = [\vec{R},\, \vec{M}(P)]$ and an axis $(\Delta)$ defined by unit vector $\vec{u}_\Delta$, for any points $P$, $Q$ on $(\Delta)$: $$ \vec{M}(P) = \vec{M}(Q) + \vec{R} \wedge \overrightarrow{QP} $$ Taking the dot product with $\vec{u}_\Delta$: $$ \vec{M}(P) \cdot \vec{u}_\Delta = \vec{M}(Q) \cdot \vec{u}_\Delta $$ so $$ \vec{M}(P) \cdot \vec{u}_\Delta = \vec{M}(A) \cdot \vec{u}_\Delta $$ The value $\vec{M}(A) \cdot \vec{u}_\Delta$ is called the **vectorial invariant** of the wrench $[W]$ with respect to axis $(\Delta)$. The **absolute vectorial invariant** is defined as: $$ \vec{j} = \frac{[\vec{R}, \vec{M}(A)] \cdot \vec{R}}{||\vec{R}||^2} $$
- **Central Axis of a Wrench:**
	The **central axis** of a wrench $[W]_P = [\vec{R},\, \vec{M}(P)]$ is the set of points $P$ for which the moment vector $\vec{M}(P)$ is collinear with the resultant $\vec{R}$: $$ \Delta = \left\{~ P ~\middle|~ \vec{M}(P) = \lambda \vec{R},\ \lambda \in \mathbb{R} ~\right\} $$ Or equivalently: $$ \Delta = \left\{~ P ~\middle|~ \vec{R} \wedge \vec{M}(P) = \vec{0} ~\right\} $$ From the fundamental relation: $$ \vec{M}(P) = \vec{M}(O) + \vec{R} \wedge \overrightarrow{OP} $$ where $O$ is a reference point. The set of points $P$ on the central axis is given by: $$ \overrightarrow{OP} = \frac{\vec{R} \wedge \vec{M}(O)}{||\vec{R}||^2} + \alpha \vec{R},\qquad \alpha \in \mathbb{R} $$
- **Operations on Wrenches:**
	The set of wrenches defined in space is a 6-dimensional vector space.
	- **Equality of Two Wrenches:**
		Two wrenches $[W_1]_P = [\vec{R}_1,\, \vec{M}_1(P)]$ and $[W_2]_P = [\vec{R}_2,\, \vec{M}_2(P)]$ are equal if and only if there exists a point $A$ such that: $$ \vec{R}_1 = \vec{R}_2 \qquad \vec{M}_1(A) = \vec{M}_2(A) $$ More generally, two wrenches are equal if, for three non-aligned points $P_1, P_2, P_3$: $$ \vec{M}_1(P_1) = \vec{M}_2(P_1) \\ \vec{M}_1(P_2) = \vec{M}_2(P_2) \\ \vec{M}_1(P_3) = \vec{M}_2(P_3) $$
	- **Sum of Two Wrenches:**
		The sum of two wrenches $[W_1]$ and $[W_2]$ is: $$ [W] = [W_1] + [W_2] \iff [W] = [\vec{R}_1 + \vec{R}_2,\, \vec{M}(P) = \vec{M}_1(P) + \vec{M}_2(P)] $$
	- **Scalar Multiplication:**
		Multiplying a wrench $[W] = [\vec{R},\, \vec{M}(P)]$ by a scalar $\lambda$ yields: $$ [\lambda W] = [\lambda \vec{R},\, \lambda \vec{M}(P)] $$
	- **Null Wrench:**
		A null (zero) wrench has $\vec{R} = \vec{0}$ and $\vec{M}(P) = \vec{0}$.
	- **Product of Wrenches:**
		Given $[W_1] = [\vec{R}_1,\, \vec{M}_1(P)]$ and $[W_2] = [\vec{R}_2,\, \vec{M}_2(P)]$, their comoment product is: $$ [W_1] \otimes [W_2] = \vec{R}_1 \cdot \vec{M}_2(P) + \vec{R}_2 \cdot \vec{M}_1(P) $$ This scalar is independent of the chosen point $P$.
	- **Derivative of a Wrench:**
		If $[\vec{R}(t),\, \vec{M}(t)]$ are functions of time, the derivative wrench is: $$ \frac{d[W]}{dt} = \left[ \frac{d\vec{R}}{dt},\, \frac{d\vec{M}}{dt} \right] $$
- **Special Wrenches: Glisser:**
	- **Glisser**
		A glisser wrench $[W]_P = [\vec{R},\, \vec{M}(P)]$ has $\vec{R} \neq \vec{0}$ and zero scalar invariant. There exists a point $A$ such that: $$ \vec{M}(A) = \vec{0} $$ At any point $P$, $$ \vec{M}(P) = \vec{R} \wedge \overrightarrow{AP} $$
	-  **Couple Wrench:**
		A nonzero wrench $[W]_P = [\vec{R}, \vec{M}(P)]$ is a couple wrench if and only if: $$ \vec{R} = 0 \qquad \exists\, A:\ \vec{M}(A) \neq 0 $$ More generally, a couple wrench may satisfy one of the following properties: 
		1. Its resultant $\vec{R} = 0$. 
		2. Its moment $\vec{M}(P)$ is uniform. 
		3. It is the sum of two attached, antiparallel vectors: $$(A, \vec{W}_1),\ (B, \vec{W}_2)\quad \vec{W}_1 + \vec{W}_2 = 0$$
	-  **General Wrench:**
		A wrench $[W]_P = [\vec{R}, \vec{M}(P)]$ is general if and only if its scalar invariant is not zero. 
		- If the scalar invariant is zero, the wrench is either a glisser or a couple wrench. 
		- If the resultant is not zero, the wrench is a glisser.
- **Decomposition of a Wrench:**
	Any wrench at point $A$, $[W]_A = [\vec{R},\, \vec{M}(A)]$, can always be written as the sum of a glisser and a couple: $$ [W]_A = [\vec{R},\, \vec{M}(A)] = [\vec{R},\, \vec{0}] + [\vec{0},\, \vec{M}(A)] $$ Here: 
	- $[G_A]$ is a glisser (sliding vector) with axis $(A,\vec{R})$, 
	- $[C(A)]$ is a couple. This decomposition is unique.

---
## 📝 Notes
- $\vec{U} \wedge \vec{V}$ is a vector orthogonal to $\vec{U}$ and $\vec{V}$, and its magnitude is$$
\left|\vec{U} \wedge \vec{V}\right| = \left|\vec{U}\right| \left|\vec{V}\right| \sin (\vec{U}, \vec{V})
$$
- $\vec{U} \cdot \vec{V} = 0 \iff \text{ the two vectors are orthogonal.}$
-  An **antisymmetric** vector field is **equiprojective**, and **vice versa**.
- We can write $W_1 = [X_1,\ Y_1,\ Z_1,\ L_1,\ M_1,\ N_1]$ $\rightarrow [W_1] \otimes [W_2] = X_1 L_2 + Y_1 M_2 + Z_1 N_2 + X_2 L_1 + Y_2 M_1 + Z_2 N_1$.

---
## Examples
#### Single Attached Vector:
For an attached vector $(A, \vec{W})$, the associated antisymmetric moment field at any point $P$ is: $$ \vec{M}_A(P) = \vec{W} \wedge \overrightarrow{AP}, \qquad \vec{M}_A(A) = \vec{0} $$ The associated wrench is: $$ [W]_A = [\vec{W},\, \vec{M}_A(P)] $$
#### Finite Set of Attached Vectors:
For $(A_i, \vec{W}_i)$, $i=1,\,\ldots,\,N$: - The associated wrench is: $$ [W] = \sum_{i=1}^N [\vec{W}_i,\, \vec{W}_i \wedge \overrightarrow{A_iP}] $$
- The moment at any point $P$: $$ \vec{M}(P) = \sum_{i=1}^N \vec{W}_i \wedge \overrightarrow{A_iP} $$
- The resultant is: $$ \vec{R} = \sum_{i=1}^N \vec{W}_i $$
- At any other point $O$: $$ \vec{M}(O) = \sum_{i=1}^N \vec{W}_i \wedge \overrightarrow{A_iO} $$ If $\vec{R} = \vec{0}$, then the wrench is a couple.

