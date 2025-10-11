---
aliases:
  - chapter_I
---

## 📚 Course Structure
- Section 1: **Random Experiments**
- Section 2: **probability spaces**
- Section 3: **Conditional Probability**
- Section 4: **Independence of Events**
---
## 📐 Equations & Concepts
#### Random Experiments
a random experiment is all experiments where we cannot know the result before it happens.
- **universal set:**
	the universal set of a random experiment is the set $\Omega$ of all possible results of the experiment.
- **Events:**
	An event is any subset of the sample space (the set of all possible outcomes) to which a probability can be assigned.
	The set of all subsets of $\Omega$, that is, the set of all events, is denoted $P(Ω)$.
- **Notion Of Probability:**
	To try to "measure" this chance, we must repeat the experiment several times. If the experiment is repeated $n$ times, we count the number $r$ of times that event $A$ occurs. The ratio $nr$ is called the frequency of occurrence of $A$, or the frequency of $A$, and is denoted by $f(A)=\frac{r}{n}$.
	Here are the properties satisfied by ff:
	- $f(A)∈[0;1]$
	- If $A$ and $B$ are two incompatible events, then $f(A∪B)=f(A)+f(B)$
	- $f(A)=1−f(\bar{A})$
	- $f(Ω)=1$ and $f(∅)=0$
	Intuitively, as $n$ tends towards $\infty$, $f(A)$ approaches a finite limit. This limit is called the probability of $A$ and is denoted $P(A)$.  

#### Probability Spaces
- **finite probability spaces:**
	let $\Omega$ and $P(\Omega)$, the couple $(\Omega,P(\Omega))$ is called a **probabilisable space**.
	Let $(Ω,P(Ω))$ be a probabilisable space. A probability defined on this space is any function $P$ from $P(Ω)$ to $[0;1]$ that satisfies:
	- $P(Ω)=1$
	- If $A$ and $B$ are two incompatible events, then $P(A∪B)=P(A)+P(B)$.
	The **triplet $(Ω,P(Ω),P)$** is called a **finite probability space**, and for any event $A$, the real number $P(A)$ is called the **probability of the event $A$**.  
- **General Case:**
	When the sample space $Ω$ is infinite, constructing a probability can be more complex than with a finite sample space. For some experiments , $Ω$ can be countably infinite $(\mathbb{N}^∗)$. For geometric or continuous spaces, calculating probabilities might involve areas, and not all sets can be measured in practice. Thus, one focuses on subsets for which probability can be assigned.
	- **Tribu $\sigma$-algebra:**
		a $\sigma$-algebra $\mathcal{A}$ on a set $\Omega$ is a collection of subsets of $\Omega$ such that:
		- $\Omega \in \mathcal{A}$
		- If $A \in \mathcal{A}$, then $\bar{A} \in \mathcal{A}$
		- For any countable family $(A_i)_{i \in \mathbb{N}} \subset \mathcal{A}$, $\bigcup_{i \in \mathbb{N}} A_i \in \mathcal{A}$
		Given a set $\Omega$ and a sigma-algebra , the pair $(\Omega, \mathcal{A})$ is called a probabilisable space. When paired with a probability $P$, the triplet $(\Omega, \mathcal{A}, P)$ is a **probability space**.
	- **Probability Space:**
		Let $(\Omega, \mathcal{A})$ be a probabilisable space. A probability on $(\Omega, \mathcal{A})$ is any function $P$ from $\mathcal{A}$ into $[0,1]$ such that:
		- $P(\Omega) = 1$.
		- If $(A_n)_{n \in \mathbb{N}}$ is a sequence of pairwise incompatible events, then: $$ P\left( \bigcup_{n=0}^{+\infty} A_n \right) = \sum_{n=0}^{+\infty} P(A_n) $$The triple $(\Omega, \mathcal{A}, P)$ is then called a probability space.
		The main difference from the finite case is that, for the second property, it is necessary to consider an infinite sequence of events---which is not possible in the finite case because there are only finitely many events.
- **Properties:**
	- An event $A \in \mathcal{A}$ is called negligible if $P(A) = 0$ and almost sure if $P(A) = 1$.
	- Let $(\Omega, \mathcal{A}, P)$ be a probability space and let $A$ and $B$ be two events.
		- $P(\bar{A}) = 1 - P(A)$, so $P(\varnothing) = 0$ 
		- $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
		- If $A \subset B$ then $P(A) \leq P(B)$
		- $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
	- **Poincaré's Sieve Formula:**
		Let $(\Omega, \mathcal{A}, P)$ be a probability space. For any family $(A_i)_{1 \leq i \leq n}$ of events: $$ P\left(\bigcup_{i=1}^n A_i\right) = \sum_{k=1}^{n} (-1)^{k+1} \sum_{1 \leq i_1 < \cdots < i_k \leq n} P(A_{i_1} \cap \cdots \cap A_{i_k}) $$
- **Elementary Events:**
	In the case where $\Omega$ is finite: $\Omega = \{\omega_1, \ldots, \omega_n\}$ The events $\{\omega_i\}$ are called elementary events.
	- Let $(\Omega, P(\Omega), P)$ be a finite probability space. For any event $A$, we have: $$P(A) = \sum_{\omega_i \in A} P(\{\omega_i\})$$
	- **Equiprobable Elementary Events:**
		Two events are called equiprobable if they have the same probability. If all elementary events are equiprobable, then necessarily $P(\{\omega_i\}) = \frac{1}{n}$, therefore, any event $A$: $$P(A) = \sum_{\omega_i \in A} P(\{\omega_i\}) = \frac{\mathrm{card}(A)}{n}$$
- **Complete System of Events:**
	- Let $(\Omega, \mathcal{A})$ be a probabilisable space. A collection $\{A_i\}_{i \in I}$ of elements of  (where $I$ is a subset of $\mathbb{N}$) is called a complete system of events if:
		- The events $A_i$ are pairwise incompatible.
		- $\Omega = \bigcup_{i\in I} A_i$
	- Let $(\Omega, \mathcal{A}, P)$ be a probability space and $\{A_i\}_{i \in I}$ a complete system of events. Then: $$\sum_{i\in I} P(A_i) = 1$$
- **Monotone Limit Property:**
	- Let $(\Omega, \mathcal{A}, P)$ be a probability space.
		- If $(A_n)_{n \in \mathbb{N}}$ is an increasing sequence of events in $\mathcal{A}$ (i.e., $A_n \subset A_{n+1}$), then $\left(P(A_n)\right)_{n \in \mathbb{N}}$ converges and: $$P\left(\bigcup_{n=0}^{+\infty} A_n\right) = \lim_{n \to +\infty} P(A_n)$$
		- If $(A_n)_{n \in \mathbb{N}}$ is a decreasing sequence of events in $\mathcal{A}$ (i.e., $A_{n+1} \subset A_n$), then $\left(P(A_n)\right)_{n \in \mathbb{N}}$ converges and: $$P\left(\bigcap_{n=0}^{+\infty} A_n\right) = \lim_{n \to +\infty} P(A_n)$$
	- Let $(\Omega, \mathcal{A}, P)$ be a probability space. If $(A_n)_{n \in \mathbb{N}}$ is a sequence of events in $\mathcal{A}$:
		- $$P\left(\bigcup_{k=0}^{+\infty} A_k\right) = \lim_{n \to +\infty} P\left(\bigcup_{k=0}^{n} A_k\right)$$
		- $$P\left(\bigcap_{k=0}^{+\infty} A_k\right) = \lim_{n \to +\infty} P\left(\bigcap_{k=0}^{n} A_k\right)$$

#### Conditional Probability
- Let $(\Omega, \mathcal{A}, P)$ be a probability space and $A$ an event with nonzero probability. For any event $B$:$$P_A(B) = \frac{P(A \cap B)}{P(A)}$$
$P_A$ is a probability on $(\Omega, \mathcal{A})$, called conditional probability relative to $A$ or probability given $A$. $P_A(B)$ is sometimes written $P(B/A)$.
- **Formulas:**
	Let $(\Omega, \mathcal{A}, P)$ be a probability space and $I$ a subset of $\mathbb{N}$.
	- **Formula for Compound Probabilities:**
		Let $(A_i)_{1 \leq i \leq n}$ be a family of events with $P(A_1 \cap A_2 \cap \cdots \cap A_{n-1}) \neq 0$. Then: $$P\left( \bigcap_{k=1}^n A_k \right) = P(A_1) P_{A_1}(A_2) P_{A_1 \cap A_2}(A_3) \cdots P_{A_1 \cap \cdots \cap A_{n-1}}(A_n)$$
	- **Formula of Total Probability:**
		Let $(A_i)_{i \in I}$ be a complete system of events with nonzero probabilities. For any event $B$: $$P(B) = \sum_{i \in I} P(A_i \cap B) = \sum_{i \in I} P(A_i) P_{A_i}(B)$$
	- **Bayes' Formula:**
		Let $(A_i)_{i \in I}$ be a complete system of events with nonzero probabilities, and $B$ an event with nonzero probability. For any $i_0 \in I$: $$P_B(A_{i_0}) = \frac{P(A_{i_0}) P_{A_{i_0}}(B)}{\sum_{i \in I} P(A_i) P_{A_i}(B)}$$

#### Independence of Events
- **Definition:**
	Two events $A$ and $B$ are said to be independent for the probability $P$ if: $$P(A \cap B) = P(A) \times P(B)$$ Then $P_A(B) = P(B)$ and $P_B(A) = P(A)$.
- If $A$ and $B$ are independent, then $\overline{A}$ and $B$, $A$ and $\overline{B}$, $\overline{A}$ and $\overline{B}$ are also independent.
- **Definition:**
	Let $A_1, \ldots, A_n$ be $n$ events.
	- The events are called pairwise independent for $P$ if $\forall\ i \neq j,\ A_i$ and $A_j$ are independent.
	- The events are called mutually independent for $P$ if for any non-empty subset $I$ of $\{1, \ldots, n\}$: $$P\left( \bigcap_{i\in I} A_i \right) = \prod_{i\in I} P(A_i)$$
- If $A_1,\ldots,A_n$ are independent for $P$, then any selection of them $B_1,\ldots,B_n$, with $B_i = A_i$ or $B_i = \overline{A_i}$, is a mutually independent family for $P$.
- **Definition:**
	If $(A_n)_{n \in \mathbb{N}}$ is an infinite sequence of events, they are independent for $P$ if for every finite subset $I$ of $\mathbb{N}$: $$P\left( \bigcap_{i\in I} A_i \right) = \prod_{i\in I} P(A_i)$$
- Let $(A_n)_{n \in \mathbb{N}}$ be an infinite sequence of independent events. Setting $B_n = \bigcap_{i=0}^n A_i$ or $B_n = \bigcup_{i=0}^n A_i$, the sequence $(B_n)_{n \in \mathbb{N}}$ is also a sequence of mutually independent events for $P$.

---
## 📝 Notes
- Certain event: represented by $\Omega$.
- Impossible event: represented by $\emptyset$.
- Events that are represented by a singleton $\{ω\}$ are called **elementary events**.
- the **elements of $\mathcal{A}$** are **Events**.
- Any **countable union or intersection of sets** in $\mathcal{A}$ is still in $\mathcal{A}$.




