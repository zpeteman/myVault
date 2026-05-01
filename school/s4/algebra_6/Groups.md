---
aliases:
  - Chapter_I
---
## 📚 Course Structure
- Section 1: **internal composition law** 
- Section 2: **groups**
- Section 3: **Sub-Groups**
- Section 4: **Morphism** 
- Section 5: **Bounded Sub-Groups**
- Section 6: **Modular & Lagrange Theorem**
- Section 7: **Isomorphism Theorem**
- Section 8: **Group to set**
- Section 9: **Groups $S_n$ and $A_n$** 
 
---
## 📐 Equations & Concepts
#### internal composition Law :
**Definitions**
- **internal composition Law**
	Let $E$ be a set, an internal composition law $*$ is an application from $E \times E$ to $E$ s.t $(x,y) \in E \times E \to x*y \in E$.
- Let $*$ be a law in $E$. we say :
	- $*$ is commutative if $\forall x,y \in E ; x*y = y*x$
	- $*$ is associative if $\forall x,y,z \in E ; x* (y*z)= (x*y)*z$
	- $*$ have $e(\in E)$ for neutral neutral if $\forall x \in E, x*e=e*x=x$ 
- Let $(E,*)$ be a set with the internal law $*$. we say that $(E,*)$ is a monoide if the law $*$ is associative and have a neutral element.
- Let $(E,*)$ a monoide. we note $e$ the neutral element. let $x \in E$, x is symmetrical if $x*x'=x'*x=e$ 
- Let $\forall a,b \in E, (a*x =b*x \implies a=b) \text{ and } (x*a= x*b \implies a=b)$
**Proprites:**
- Let $(E,*)$ and ljjet $A$, we say that $A$ is stable by $*$ if $\forall (x,y) \in A^2, x * y \in A$.
- $x$ and $y$ are symmetrical then $(x*y)' = y'*x'$
#### Groups
**Definitions**
- Let $(G,*)$ be a group if and only if:
	- $*$ be associative.
	- $*$ have a neutral element.
	- all $G$ elements are symmetrical.
	if $*$ is commutative then $(G,*)$ is abelien.
- Let $(G,*)$ be finite if $G$ is finite. the cardinal of $G$ is $|G|$ or $o(G)$.
- Let $(G_1,*)$ and $(G_2,T)$. $G_1 \times G_2$ is defined by the law $\bot$, $(x_1,x_2)\bot(y_1,y_2)=(x_1*y_1,x_2Ty_2)$. $G_1 \times G_2$ is a group called product group. the neutral $(e_{G_1},e_{G_2})$ the symmetrical of $(x_1,x_2)$ is $(x_1',x_2')$. 

#### Sub-Groups
**Definitions**
- Let $(G,.)$ and $H$ a part of $G$. we say that $H$ is a sub-group of $(G,.)$ if 
	- $H$ is stable by the law $.$ $\forall x,y \in H, x.y \in H$
	- the induit law, $(H,.)$ is a group.

**Propositions**
- $H$ is a sub-group of $(G,.)$ then we have :
	- the neutral element of $(H,.)$ is a neutral element of $(G,.)$
	- the symmetrical element $x$ of $H$ in $(H,.)$ is the same in $(G,.)$
- Let $(G,.)$ a group and $H$ be a part of $G$.
	- $H$ is a sub group of $(G,.)$
	- 
		- $H \ne \emptyset$
		- $\forall x,y \in H, x.y \in H$
		- $\forall x \in H, x^{-1} \in H$
		- $\forall x,y \in H , x.y^{-1} \in H$
- Let $(G,.)$ 
	- Let $H$ and $H'$ be sub groups of $G$. the $H\cap H'$ is a subgroup of $G$.
	- Let $(H_i)_{i\in I}$ is a family of sub groups of $G$. then $\bigcap_{i \in I} H_i$ is a subgroup of $G$.

#### Morphism
**Definitions**
- Let $(G_1,.)$ and $(G_2, .)$, and application $f: G_1 \to G_2$ is a morphism of groups if for all $x,y \in G_1$, we have $f(x.y) = f(x).f(y)$.

**Propositions**
-  Let $f: (G,.) \to (G_2, .)$ is a morphism then $f(e_{g_1}) = e_{g_1}$ if for all $x \in G_1$, we have $(f(x))^{-1}=f(x^{-1})$.
- Let $f:(G_1,.) \to (G_2,.)$ is a morphism
	- $f$ is injective $\iff Kerf = {e_{G_1}}$.

### bounded sub-group
**Definitions**
- Let $A$ be a part of $(G,.)$. we note $\epsilon_A$ the set of sub groups of $G$ with $A$, we pose $<A> = \bigcap_{H\in \epsilon_A} H$, then $<A>$ is a sub group of $G$ having $A$ as an element and it's the smallest subset containing $A$, we call $<A>$ is the bounded subset $A$.
- df
	- Let $(G,.)$ is monogene if it's bounded by a part of one element.
	- a group is cyclic if it's monogene and finite.
- Let $G$ is a group $a \in G$. we save that $a$ is a finite order if $<a>$ is finite. i this case, we call order of $a$, noted $o(a)$ or $|a|$, the order of $<a>$.
**Propositions**
- Let $(G,.)$ be a group and $a \in G$  then $<a>=\{a^n / n \in \mathbb{Z}\}$ 

**Theorems**
- Let $(G,.)$ is a neutral element $e$ and $a \in G$. then $a$ is a finite order if and only if there's $n \in \mathbb{N}^*$ st $x^n =e$ then $o(a)= min\{k \in \mathbb{N}^* / a^{k}=e\}$. plus we have $<a>={e,a,a^2, \dots , a^{s-1}}$ where $s=o(a)$.

#### Modular and Lagrange theorem
**Definitions**
- Let $(G,.)$ be a group and $H$ a subgroup of $G$. we define $\mathcal{R}_g$ in $G$ by:$\forall x, y \in G, x \mathcal{R}_g y \iff x^{-1}.y \in H$ $\mathcal{R}_g$ is an equivalence relationship called equivalence in left modular $H$. if $x\in G$, we note $\bar{x}^g$ is an equivalence for $\mathcal{R}_g$, called the left class modular $H$ $\bar{x}^g=x.H$
**Propositions**
**Theorems**
- **Lagrange Theorem**
	Let $(G,.)$ be a finite group and $H$ is a sub group of $G$ then $|G|=|H|.[G:H]$ in particular the order of $H$ divide the order of $G$.
- Let $(G,.)$ be a finite group. $\forall x \in G$ we have $card(x.H) = card (H)$.
- $(G,.)$ is finite of order $n$, with neutral element $e$. then for all $x$ in $E$, we have $o(x)/n$. in particular $x^n = e$ 

#### Isomorphism Theorem
- **distinct sub-groups**
	**Definitions**
	- Let $(G,.)$ be a group and $H$ a sub-group of $G$. we say that $H$ is a sub group different of $G$ we note $H\nabla G , \forall x\in G , x.H =H.X$.
	**Propositions**
	- Let $(G,.)$ a group, $H$ a sub-group of $G$ is different if and only if $\forall x \in G, x H x^-1 \subset H$.
- **quotient of group**
	**Theorems**
	- Let $(G,.)$ be a group with neutral element $e$ and $N$ a sub-group distinct of $G$. Then in the quotient set $G/N$ , e define the law $\odot$ for all $x,y \in G$ $\bar{x}\odot \bar{y} = \bar{xy}$ $G/N$ have $\bar{e}$ as neutral element and the surjective canonic $\Pi: G \to G/N$ is a morphism of groups , if $G$ is abelien, then $G/N$ is abelien if $G$ is finite, $G/N$ is finite and we have $|G/N|=\frac{|G|}{|N|}$.
- **isomorphism theorem and applications**
	**Theorems**
	-  **Decomposition**
		Let $E,F$ be two sets $f: E \to F$ and $\mathcal{R}$ an equivalence relationship and $\Pi: E \to E/\mathcal{R}$ we suppose $\forall x,y \in E x \mathcal{R} y \implies f(x) =f(y)$ then there exist a unique $\bar{f}: E/ \mathcal{R} \to F$ s.t $f=\bar{f} \circ \Pi$, $\forall x,y \in E ,x \mathcal{R} y \iff f(x) = f(y)$ then $\bar{f}$ is injective.   
	- **First isomorphism theorem**
		Let $f: G \to G'$ and $N$ a distinct sub-group of $G$ such that $C \subset Kerf$then there exists a morphisme $\bar{f}: G/N \to G'$ s.t $\forall x \in G, f(x) = \bar{f}(\bar{x})$, if $N = Kerf$ then $\bar{f}$ is an injective morphism. and the application $\bar{f}: G/Ker f \to Im f$ is an isomorphism ($G/Kerf \cong Imf$).
	- **Second isomorphism theorem**
		Let $(G,.)$ is a group, $H, N$ two sub-groups of $G$ with $N$ distinct in $G$ then $HN$ is a sub group of $G$ and we have $HN/N \cong H/H\cap N$ in particular if $H$ and $N$ are finite then $|HN| |H\cap N| = |H||N|
	- **Characteristics of direct product**
		Let $G$ be a group :
		- $G \cong G_1 \times \dots \times G_n$
		- $G$ contains $n$ distinct sub groups $H_1, \dots , H_n$ s.t
			- $G_i \cong H_i$
			- $\forall x \in G, \exists(x_1,\dots, x_n) \in H_1 \times \dots \times H_n$ unique s.t $x = x_1 \dots x_n$.
	- Let $G$ be a group :
		- $G \cong G_1 \times G_2$
		- $G$ contains two sub-groups $H_1$ and $H_2$ s.t :$G_1 \cong H_1, G_2 \cong H_2, G = H_1H_2 , H_1 \cap H_2 = \{e\}$.
	- **Third isomorphism theorem**
		Let $G$ and $N$ be a distinct sub-group of $G$. then the supgroups $G/N$ are exactly of the form $H/N$, wher $H$ is then sub group of $G$ containing $N$. and $H/N$ is distinct in $G/N$ if and only if $H$ is distinct in $G$ we have then $\frac{G/N}{H/N} \cong G/H$ 
	**Propositions**
	- **classifications**
		Let $G$ is a monogene group. is an infinite, it is an isomorph in $\mathbb{Z}$. if it's finite of order $n$ it is isomorphe in $\mathbb{Z}/n\mathbb{Z}$.
	- all group order a prime number it's cyclic and isomorphic in $\mathbb{Z}/p\mathbb{Z}$.
	- if $H$ and $K$ are two sub groups of $G$ $HK$ is a sub group of $G$ if and only if $HK = KH$, in particular if one of those groups are distinct in $G$ then $HK$ is a sub group in $G$.
	- all sub-groups of the cyclic graph is cyclic. and all quotient of a cyclic group is cyclic.
	- Let $G$ be a finite set of operations in the set $E$. then for all $x \in E, obr(x)$ have a finite cardinal and it's equal to $[G;G_x]$.
	- **First classes formula**
		Let $G$ be a finite group operating in the left in a finite set $E$, then we have $card E = card E^G + \sum_{s\in S /E^G}[G:G_x]$ 
	- **Second formula of classes**
		Let $G$ be a finite group then we have $|G|=|Z(G)| + \sum_{x\in S / Z(G)} [G:G_x]$ where $G_x$ is the centralist of $x$ and $S$ is the system represented of conjugation classes of $G$. 

#### group operations 
**Definitions**
- we call left operation of $G \to E$ all application $G \times E \to E (s,x) \to s.x$ s.t 
	- $s.(t.x) = (s.t).x$
	- $e.x = x$

#### Groups $S_n, A_n$
**Definitions**
- Let $E$ be a set, a permutation in $E$ is a bijection of $E$ in $E$.
- we suppose that $card E = n$, then the group of permutations for the compositions law is the symmetry group $S_n(E)=S_n$ it a group of order $n$.
- Let $\omega$ and $\sigma$ be two permutations we say that for any intersection if we have $\mathcal{S}_{\sigma} \cap \mathcal{S}_{\omega} = \emptyset$. 

**Propositions**
- Let $\sigma$ be a cycle, $\sigma \ne Id$ then the order of $\sigma$ is equal to it's length.
- if $\omega$ and $\sigma$ are distinct then $\omega \cerc \sigma = \sigma \cerc \omega$ 




---
## 📝 Notes
- $(E,*)$ is a set related to $*$.
- automorphism = isomorphism + endomorphism
- the image of $f$ is $Imf$  
- $f$ is surjective $\iff Imf=G_2$.
- if $G=<A>$, we say that $G$ is bounded by $A$. and $A$ is generatrice of $G$.
- all group of an order prime number is cyclic, bounded by whatever number different than the neutral element.