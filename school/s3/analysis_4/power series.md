---
aliases:
  - Chapter_III
---
## 📚 Course Structure
- Section 1: **Definition** 
- Section 2: **Radius Laws**
- Section 3: **Operations**
- Section 4: **Real power series**
- Section 5: **Integration**

---
## 📐 Equations & Concepts
#### Definition :
- we call a series a **power series* it it's a series of function $\sum f_n$ such that $f_n(z)=a_n z^n$, where $(a_n)$ is a complex sequence of complex numbers.
	we note is $\sum a_n z^n$.
- we call the domain of convergence the set of all $z \in \mathbb{C}$ such that the series converges. we obviously have 0 in that set.
	we note it $D_c$.
- **Abel's Lemme**:
	if $|a_n|r^n, r \in \mathbb{R}^+$ is bunded, and $|z|<r , z \in \mathbb{C}$  then the series $\sum a_n z^n$ does converge absolutely.
- let $\sum a_n z^n$ of convergence radius $R$. then, for all $z \in \mathbb{C}$ we have 
	- if $|z|<R$ then the series converge absolutely.
	- if $|z| > R$ then the series diverges trivially.
	- if $|z| = 0$ then we conclude nothing.

#### Radius Laws :
- **Alembert's Law :**
	we suppose that $\lim_{\infty} |\frac{a_{n+a}}{a_n}|=l\in [0, \infty]$ then $R= \frac{1}{l}$.
- **Cauchy's Law :**
	we suppose that $\lim_{\infty} \sqrt{|a_n|}=l\in [0, \infty]$ then $R= \frac{1}{l}$.

#### Operations :
- **Sum :** $\sum_0^{\infty} (a_n + b_n) z^n = \sum_0^{\infty}a_n z^n + \sum_0^{\infty} b_n z^n$, with $R = min(R_a; R_b)$. 
- **multiplication by a scalar :** $\sum_0^{\infty} (\lambda a_n)z^n = \lambda \sum_0^{\infty}a_n z^n$, with $R = R_a$.
- **Cauchy product :** $c_n = \sum_{k=0}^{n}a_kb_{n-k}$ which gives us $\sum_0^{\infty} c_n z^n = \sum_0^{\infty}a_n z^n \times \sum_0^{\infty}b_n z^n$. 

#### Real power series :
- let $\sum a_n x^n$ with radius $R$ and $0 < \rho < R$ then the series converge normally in all $[-\rho, \rho]$.
- let $\sum a_n x^n$ with radius $R$ and then the sum $f$ is continues in  $[-R, R] \to \mathbb{R}$.
- if $\sum a_n x^n$ then $f'(x) = \sum_1^{\infty} na_n x^{n-1},f^{(k)}(x) = \sum_0^{\infty} \frac{(n+k)!}{n!} a_{n+k} x^{n}$. and we can conclude that $a_n = \frac{f^{(n)}(0)}{n!}$.
-  let $\sum a_n x^n$ and $\sum b_n x^n$ be two series with $R_a, R_b$ and with sum $f,g$ we have:
	- $\forall x \in ]- min(R_a;R_b),min(R_a;R_b)[, f(x) = g(x) \Leftrightarrow a_n =b_n: \forall n\in \mathbb{N}$.
	- $f$ is even $\Leftrightarrow a_{2n+1} = 0, \forall n \in \mathbb{N}$.
	- $f$ is odd $\Leftrightarrow a_{2n} = 0, \forall n \in \mathbb{N}$.

#### Integration :
- **Def :**
	we call the anti-derivative of a power series is $\sum \frac{a_n}{n+1}x^{n+1}$ in another word : $\int_0^x f(t) dt = \sum_0^{\infty} \frac{a_n}{n+1}x^{n+1}$.
- **series Development :**
	let $f : I \to \mathbb{R}$, with $0 \in I$, we can develop $f$ near 0 if there's a series with radius $R$ such that $$\forall x \in I \cap ]-R, R[, f(x) = \sum_0^{\infty} a_n x^n $$
- **Conditions :**
	-  series Development conditions$$
		\begin{cases}
		& f \text{ is a } \mathcal{C}^{\infty} \text{ function near } 0. \\
		& f(x) = \frac{f^{(n)}(0)}{n!} x^n.
		\end{cases}
		$$ 
	- Taylor series conditions $$
 	\begin{cases}
 	& f \text{ is a } \mathcal{C}^{\infty} \text{ in I } \\
 	& \exists M > 0: \forall k \in \mathbb{N}; sup_{x\in I} |f^{(k)}(x)| \le M.
 	\end{cases}
 	$$
---
## 📝 Notes
- from **Abel's Lemme** we conclude that the opened disc $D(0,r[=\{z \in \mathbb{C}/|z|<r \}$ is included in $D_c$.
- $A=\{r \le 0 / (|a_n|r^n) is bounded\}, R= supA$.
- if we have two series with sequences $a_n$ and $b_n$ then: $$\begin{cases}&|a_n| = O(|b_n|) &\implies & R_a \le R_b \\&|a_n| \sim|b_n| &\implies & R_a = R_b\end{cases}$$
- a series and it's derivative and anti-derivative series all of them have the same radius always.