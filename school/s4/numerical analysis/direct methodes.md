---
aliases:
  - Chapter_I
---
## 📚 Course Structure
- Section 1: **Cramer Method** 
- Section 2: **triangular systems**
- Section 3: **Gauss Method**
- Section 4: **Pivot Method**
 
---
## 📐 Equations & Concepts
#### Cramer Method:
we know that when a matrix $A$ is inversible the the solution exists and it's unique, teh solution is giving by $X=A^{-1}B$
with $$x_i = \begin{vmatrix}a_{1,1} & \dots & a_{1,i-1} & b_1 & a_{1,i+1}& \dots &a_{1,n} \\ a_{2,1} & \dots & a_{2,i-1} & b_2 & a_{2,i+1} &\dots &a_{2,n} \\ \vdots & \ddots & \ddots & \vdots & \ddots &\ddots & \vdots \\a_{n,1} & \dots &a_{n,i-1} & b_n & a_{n,i+1} &\dots &a_{n,n} \end{vmatrix} \times \frac{1}{detA}$$
#### triangular systems
Let the system be a triangle this time and let's call it $A$. we use $AX = B$ which gives us $x_n$ :
$$
\begin{equation}
\left\{\begin{split}
 & x_n=\frac{b_n}{a_{n,n}}  \\
 & x_i = \frac{1}{a_{i,i}} (b_i - \sum_{j= i +1}^na_{i,j}x_j) \\ 
\end{split}\right.
 \end{equation}
$$
for $(i= 1, \dots , n-1)$ when it's a lower triangle we have  
$$
\begin{equation}
\left\{\begin{split}
 & x_1=\frac{b_1}{a_{1,1}}  \\
 & x_i = \frac{1}{a_{i,i}} (b_i - \sum_{j= 1}^{i-1}a_{i,j}x_j) \\ 
\end{split}\right.
 \end{equation}
$$
for $(i = 2 , \dots , n)$

#### Gauss Method
this method makes us able to transform the system $AX = B$ to a triangular system let's call it $A'X = B'$ where $A'$ is an upper triangular matrix.
$$AX=b \iff
\begin{equation}
\left\{\begin{split}
 & a_{1,1}x_1 + \dots + a_{1,n}x_n = b_1 (E_1)  \\
 & a_{n,1}x_1 + \dots + a_{n,n}x_n = b_n (E_n)\\ 
\end{split}\right.
 \end{equation}
$$
- **Step 1** we suppose that $a_{1,1}\ne 0$ transforms $(S)$ to another system where $a_{i,1}=0, \forall i = 2, \dots , n$ 
the method is : the equation $(E_i)$ is remplaced by the equation $$(E_i^{2})= (E_i) - \frac{a_{i,1}}{a_{1,1}}(E_1)$$
we get another system which is equivalent to the first one 
$$
\left\{
\begin{array}{lrccll}
a_{1,1}x_1 + & a_{1,2}x_2 + & \cdots + & a_{1,n}x_n & = b_1 & \quad (E_1^{(2)}) \\
0 + & a_{2,2}^{(2)}x_2 & + \cdots + & a_{2,n}^{(2)}x_n & = b_2^{(2)} & \quad (E_2^{(2)}) \\
\vdots & \vdots \quad & & \vdots & \vdots \\
0 + & a_{n,2}^{(2)}x_2 & + \cdots + & a_{n,n}^{(2)}x_n & = b_n^{(2)} & \quad (E_n^{(2)}).
\end{array}
\right.
\quad (S^{(2)})
$$

Where the superscript $(2)$ in the system $(S^{(2)})$ indicates step 2 of the Gaussian elimination method. 
If $a_{2,2}^{(2)} \neq 0$, we transform the system $(S^{(2)})$ into another equivalent system $(S^{(3)})$ where the equation $(E_i^{(2)})$ is replaced by the equation:

$$
(E_i^{(3)}) = (E_i^{(2)}) - \frac{a_{i,2}^{(2)}}{a_{2,2}^{(2)}} (E_2^{(2)}) \quad (\forall i = 3, \cdots, n).
$$
We therefore obtain another system equivalent to $AX = B$:

$$
\left\{
\begin{array}{lrccll}
a_{1,1}x_1 + & a_{1,2}x_2 + & \cdots & + a_{1,n}x_n & = b_1 \\
0 + & a_{2,2}^{(2)}x_2 + & \cdots & + a_{2,n}^{(2)}x_n & = b_2^{(2)} \\
0 + & 0 + & a_{3,3}^{(3)}x_3 + \cdots & + a_{3,n}^{(3)}x_n & = b_3^{(3)}. & \quad (S^{(3)}) \\
\vdots & \vdots & \vdots & \vdots & \vdots \\
0 + & 0 + & a_{n,3}^{(3)}x_3 + \cdots & + a_{n,n}^{(3)}x_n & = b_n^{(3)}.
\end{array}
\right.
$$

We continue this process and finally obtain a triangular system equivalent to the starting system $AX = B$.

- **Partial pivoting method:**
We choose as pivot the element $a_{p,k}^{(k-1)}$ s.t $|a_{p,k}^{(k-1)}| = \max_{k \le i \le n} |a_{i,k}^{(k-1)}|$ and we swap rows $k$ and $p$.

- **Complete pivoting method:**
We choose as pivot the element $a_{p,l}^{(k-1)}$ s.t $|a_{p,l}^{(k-1)}| = \max_{k \le i,j \le n} |a_{i,j}^{(k-1)}|$ and we swap rows $k$ and $p$ then columns $k$ and $l$.


---
## 📝 Notes
- Cramer Method fails for large $n$ ($n \ge 20$).
- $det A = (-1)^m \Pi_{p=1}^n a_{p,p}^{(p)}$ where $m$ is the total number of permutations.
- to implement Gauss method we need $\frac{2n^3}{3}$ operations.
- Gauss Method fails for large $n$ ($n = 100$).