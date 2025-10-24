---
aliases:
  - Chapter_IV
---
## 📚 Course Structure

- Section 1: **Kinetic Torsor**
- Section 2: **Dynamic Torsor**
- Section 3: **Kinetic Energy**
- Section 4: **Force Torsor**
- Section 5: **Fundamental Principle of Dynamics**
- Section 6: **Kinetic Energy Theorem**

---

## 📐 Equations & Concepts

#### Kinetic Torsor
- **Definition**
	$$\tau_c(S/R) = [P(S/R); \sigma(S/R)]$$

	- **Momentum P(S/R):**
    - **Center of Mass:** $$P(S/R) = mV(G/R)$$
    - In barycentric frame: $P(S/R_G) = 0$
	- **Angular Momentum σ(S/R):**
	    - **Center of Mass:** $$\sigma(G; S/R) = J(G, S) \cdot \omega_{S/R}$$
	    - **Koenig's Theorem II:** $$\sigma(O; S/R) = J(G, S) \cdot \omega_{S/R} + mOG \wedge V(G/R)$$
	    - For A fixed in R: $$\sigma(A; S/R) = J(A, S) \cdot \omega_{S/R}$$
#### Dynamic Torsor
- **Definition**
	$$\tau_D(S/R) = [S(S/R); D(S/R)]$$
	- **Dynamic Resultant:** $$S(S/R) = ma(G/R) = \frac{dP(S/R)}{dt}$$
    
	- **Dynamic Moment:**
    
	    - **At center of mass G:** $$D(G/R) = \frac{d\sigma(G; S/R)}{dt}$$
	    - **At fixed point A:** $$D(A/R) = \frac{d\sigma(A; S/R)}{dt}$$
	    - **Koenig's Theorem III:** $$D(O; S/R) = D(G; S/R) + mOG \wedge a(G/R)$$
	    - **General torsor relation (when V(C/R) = 0):** $$\tau_D(C; S/R) = \frac{d\tau_c(C; S/R)}{dt}$$
#### Kinetic Energy
- **Definition**
	$$E_C(S/R) = \frac{1}{2}\int_{M \in S} dm,[V(M \in S/R)]^2$$
	- **Koenig's Theorem IV:** $$E_C(S/R) = \frac{1}{2}mV^2(G/R) + \frac{1}{2}\omega_{S/R} \cdot J(G; S/R) \cdot \omega_{S/R}$$
	    - Translation energy: $E_C^{translation}(S/R) = \frac{1}{2}mV^2(G/R)$
	    - Rotation energy: $E_C^{rotation}(S/R) = \frac{1}{2}\omega_{S/R} \cdot J(G; S/R) \cdot \omega_{S/R}$
	- **Alternative Form:** For A fixed in R: $$E_C(S/R) = \frac{1}{2}\omega_{S/R} \cdot \sigma(A; S/R) = \frac{1}{2}\omega_{S/R} \cdot J(A; S/R) \cdot \omega_{S/R}$$
	- **Torsor Product:** $$2E_C(S/R) = (\tau_C(S/R), \tau_V(S/R))$$
#### Force Torsor
- **Definition**
	$$\tau_F(S/R) = [F(S/R), M(O; S/R)]$$
	- **Resultant Force:** $$F(S/R) = \sum_{P_i \in S} F_i$$
	- **Resultant Moment (antisymmetric field):** $$M(O; S/R) = \sum_{P_i \in S} OP_i \wedge F_i$$ $$M(A; S/R) = M(B; S/R) + AB \wedge F(S/R)$$
	- **Weight Torsor:** $$\tau_P(O; S/R) = [mg, OG \wedge mg]$$ At G: $\tau_P(G; S/R) = [mg, 0]$
    
	- **Key Result:** $$\tau_F(S/R) = \tau_F^{ext}(S/R) + \tau_F^{int}(S/R)$$ $$\tau_F^{int}(S/R) = 0$$ Therefore: $\tau_F(S/R) = \tau_F^{ext}(S/R)$
    
#### Fundamental Principle of Dynamics
-  Galilean Reference Frame

$$\tau_D(S/R_0) = \tau_F^{ext}(S/R_0)$$

- **Theorem of Dynamic Resultant:** $$ma(G/R_0) = \sum_i F_i^{ext}$$
- **Theorem of Angular Momentum:** $$\frac{d\sigma(O; S/R_0)}{dt} = M_F^{ext}(O; S/R_0) = \sum_i OP_i \wedge F_i^{ext}$$
- **For rotation about fixed axis (O, u):** $$u \cdot \frac{d\sigma(O; S/R_0)}{dt} = u \cdot M_F^{ext}(O; S/R_0)$$
- **Action-Reaction Theorem:** $$\tau_F(S_2 \to S_1/R_0) = -\tau_F(S_1 \to S_2/R_0)$$

#### Non-Galilean Reference Frame

$$\tau_D(S/R) = \tau_F^{ext}(S/R) - \tau_D^{entrainment} - \tau_D^{Coriolis}$$

Where:

- $a(M \in S/R) = a(M \in S/R') + a_e(M/R) + a_c(M/R)$
- $a_e(M/R) = a(O'/R) + \frac{d\omega_{R'/R}}{dt} \wedge O'M + \omega_{R'/R} \wedge (\omega_{R'/R} \wedge O'M)$
- $a_c(M/R) = 2\omega_{R'/R} \wedge V(M \in S/R')$

---

### Section 6: Kinetic Energy Theorem

#### Power

$$P(S/R) = (\tau_v(S/R); \tau_F^{ext}(S/R))$$ $$P(S/R) = F \cdot V(A \in S/R) + \omega_{S/R} \cdot M(A; S/R)$$

- Internal forces do no work: $P^{int}(S/R) = 0$

#### Work

- **Elementary work:** $$dW(t; S/R) = P(t; S/R)dt$$
    
- **Work between $t_i$ and $t_f$:** $$W(t_i, t_f; S/R) = \int_{t_i}^{t_f} P(t; S/R)dt$$
    

#### Kinetic Energy Theorem (Galilean Frame)

$$W(t_i, t_f; S/R) = E_c(t_f; S/R) - E_c(t_i; S/R)$$

Or equivalently: $$(\tau_F^{ext}, \tau_v) = \frac{d}{dt}(E_c(t; S/R))$$

#### Perfect Connections (No Energy Loss)

- **Pivot Connection (Rotation about axis (O, Z₀)):** Perfect if: $Z_0 \cdot M(A; S/R_0) = 0$ (Moment of reaction forces perpendicular to rotation axis)
    
- **Spherical Connection (Rotation about point O):** Perfect if: $M(O; S/R_0) = 0$ (Moment of reaction forces is zero)
    
- **Sliding Connection (Translation along axis (O, Y₀)):** Perfect if: $R(S_0 \to S) \cdot V(B \in S/R_0) = 0$ (Reaction force perpendicular to sliding axis)
    

---

## 📝 Notes

- **Composite solids:** For $S = S_1 \cup S_2$ with $S_1 \cap S_2 = \emptyset$: all quantities (P, σ, E_c, τ) are additive.
- **Key points for calculations:** Use G (center of mass) or fixed points A to simplify torsor expressions.
- **Koenig's four theorems:** Central for separating translation and rotation contributions.
- **In Galilean frame:** $\tau_D = \tau_F^{ext}$ (fundamental principle).
- **Internal forces:** Always cancel out ($\tau_F^{int} = 0$, $P^{int} = 0$).
- **Perfect connections:** No energy loss means work of reaction forces is zero.
- **Power as torsor product:** $P(S/R) = (\tau_v, \tau_F^{ext})$ simplifies calculations.
- **Kinetic energy theorem:** Relates work to change in kinetic energy in Galilean frames.