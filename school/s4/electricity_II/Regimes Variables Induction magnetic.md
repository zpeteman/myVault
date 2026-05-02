---
aliases:
  - Chapter_III
---
# Faraday Induction Law
## Circuit that moves in a magnetic field constant
$$e = -\frac{d\Phi}{dt}$$
## electric field expression
$$\vec{E} = - \frac{\partial \vec{A}}{\partial t}$$
## electric field Proprieties
$$\begin{aligned} 
\vec{E} &= - \vec{grad} V - \frac{\partial \vec{A}}{\partial t} \\
&\vec{rot\vec{E}} + \frac{\partial \vec{B}}{\partial t} = \vec{0}
\end{aligned}$$
# mutual inductance of two circuits
$$\Phi_{ba} = M_{ba}l_b$$
# Auto-induction
## solenoid 
$$\vec{B} = \mu_0 n I \vec{e}_z$$
with $n=\frac{N}{l}$ 
$$\begin{aligned} 
\Phi &= N \phi = N \iint_{spire}\vec{B}d\vec{S}=N \iint_{spire}BdS \\
\Phi &= \mu_0 \frac{N^2}{l}I \pi R^2 = \mu_0 n^2 lI\pi R^2 \\
L &= \frac{\Phi}{I} = \mu_0 \frac{N^2}{l} \pi R^2 = \mu_0 n ^2 l \pi R^2
\end{aligned}$$
## toroidal coil
$$\begin{aligned}
\vec{B} &= \frac{\mu NI}{2 \pi \rho} \vec{e}_{\phi} \\
L &= \frac{\mu_0 N^2}{2\pi}b Log\left(\frac{2R+a}{2R-a}\right)
\end{aligned}$$
# transformers
$$\begin{aligned} 
u_1(t) &= r_1i_1(t) + \frac{d\Phi_1}{dt} \\
u_2(t) &= r_2i_2(t) + \frac{d\Phi_2}{dt} \\
\frac{u_2(t)}{u_1(t)} &= \frac{M}{L_1} \\
\implies \frac{M}{L_1} &= \frac{N_2}{N_1}
\end{aligned}$$
# work of the magnetic force
$$T= I. \Delta \Phi \text{ Maxwell theorem}$$
# Magnetic energy
## in function of the magnetic field $\vec{B}$
$$\begin{aligned} 
W &= \iiint \frac{B^2}{2\mu_0}dv \\
w_m &= \frac{dW}{dv} = \frac{B^2}{2\mu_0}
\end{aligned}$$
## in function of $I$ and the $\Phi$
$$W = \frac{1}{2} \sum_1^n I_i \Phi_i \text{ or } \Phi_i = \Phi_{ii} + \sum_{j \ne i} \Phi_{ji}$$


























