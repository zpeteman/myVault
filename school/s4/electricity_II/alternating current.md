---
aliases:
  - Chapter_V
---
# sinusoidal quantity
the general form is : $$x = x_0 cos(\omega t + \alpha)$$
the efficient value is given by : $$x_{eff} = \sqrt{\frac{1}{T}\int_0^1 x^2 dt} = \frac{x_0}{\sqrt{2}}$$
we have : 
- $u = u_0 cos(\omega t + \alpha)$ 
- $i = i_0 cos(\omega t + \beta)$
# linear circuits laws in an alternating current
## Ohm's law
### resistance $R$
$u_A - u_B  = R.i  = u_r$
### ideal coils
$e=- \frac{d\phi}{dt}, \phi = L.i$ and $u_A - u_B = -e = L \frac{di}{dt} = u_L$ 
### capacitors
$i=\frac{dq}{dt}, q= C u_c \implies i = C \frac{du_c}{dt} / u_c = \frac{1}{C} \int i. dt$

## Kirchhoff Law
- Noeuds Law : $\sum i = 0$
- Mailles Law : $\sum u = 0$

# complex notations
we can write $x = x_0 cos (\omega t + \alpha)$ $$\bar{x} = x_0 cos (\omega t + \alpha ) + j x_0 sin (\omega t + \alpha) = x_0 exp\left(j ( \omega t + \alpha )\right)$$
with $x$ being the real part of $\bar{x}$.
$$\frac{d\bar{x}}{dt} = j \omega \bar{x}, \int\bar{x}dt = \frac{1}{j\omega} \bar{x}$$
## complex representation of $u$ and $i$
$$\bar{u} = u_0 exp(j\alpha)$$
$$\bar{i} = i_0 exp (j \beta)$$
## Kirchhoff Law
kirchhoff laws in complex notions  gives us $\sum \bar{I} = 0$, $\sum \bar{U} = 0$ or $\sum(R+ jL\omega + \frac{1}{jC\omega})\bar{I} - \bar{E} = 0$
$\bar{E}$ represent the complex amplitudes.

# Ohm's Law 
## Ohm's Law
$$\bar{u} = \bar{Z}.\bar{i}$$
## impedance
$$\bar{Z} = \frac{\bar{U}}{\bar{I}}= \frac{\bar{u}}{\bar{i}}$$
$\bar{Z} = Z exp(j \psi)$ with $\psi = \alpha - \beta$,  $\bar{Z} = R + j X$   
with $R$ the resistance in the circuit between $A$ and $B$ ($R$ is always positive), and $X$ reactance in the circuit between $A$ and $B$ ($X$ can be positive or negative).
we also have $$\bar{Y} = \frac{1}{\bar{Z}}$$
with $\bar{Y} = G + j B$ 
with $G$ it's always positive, $B$ may be positive or negative.
# power in sinusoidal regime
## instant power - active power 
$$P = U_{eff} I_{eff} cos \phi$$
### reactive power 
$$P_r = U_{eff}I_{eff} sin \phi$$
$P_r$ is on Volt Ampere Reactivity 
### apparent power
$$P_a = U_{eff} I_{eff}$$
$P_a$ is on Volt Ampere
$P_a = \sqrt{P^2 + P_r^2}$ 
### complex power 
$$\bar{P} = \frac{1}{2} \bar{U}\bar{I}^*$$ with $\bar{U} = U_0$ and $\bar{I}^* = I_0 exp(j\phi)$ 

Let $$\bar{P} = \frac{1}{2} U_0 I_0 (cos \phi + j \sin \phi) = P + j P_r$$
we get 
$$\begin{cases}
P &= U_{eff}I_{eff} cos \phi = R_e (\bar{P}) \\
P_r &= U_{eff}I_{eff} sin \phi = I_m(\bar{P}) \\
P_a &= U_{eff}I_{eff} = |\bar{P}|
\end{cases}$$




















































































