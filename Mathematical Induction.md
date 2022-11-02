Suppose I wish to prove a [[Statement]] of the form $\forall n \in \mathbb{Z} \geq q$, $P(n)$.
1. Show $P(a)$ is true. That is, show the predicate holds for the very first element in the domain.
2. Show for all $\forall n \in \mathbb{Z}, P(n) \rightarrow P(n+1)$.  If the predicate holds true for $n \in \mathbb{Z} \geq a$, then the predicate holds true for $(n+1) \in \mathbb{Z} \geq a$.  
	- If the predicate holds true for $n$, then it holds true for the next value in the domain ($n+1$).

> ($1.+2.$) $Truth Set_p = \{x \in \mathbb{Z} \geq a | P(x) \text{ is true}\} = \{a,a+1,a+2,a+3,...\} = \mathbb{Z} \geq a$.

<b>Statement:</b> $\forall n \in \mathbb{Z} \geq a, P(n)$
1. Base Case(s)
	- Show $P(a)$ is true.
2. Inductive Step
	- Prove (usually via [[Direct Proof]]), $\forall n \in \mathbb{Z} \geq a, P(n) \rightarrow P(n+1)$.
		- Let $k \in \mathbb{Z} \geq a$ such that $P(k)$ is true.
		- The assumption that $P(k)$ is true is known as the <b>inductive hypothesis</b>.
		- From there, do some hard work to show $P(k+1)$ is true.

### Example 1
Prove that $\forall n \in \mathbb{N}, 3|(2^n-1) \equiv \forall n \in \mathbb{Z} \geq 1, 3|(2^n-1)$.

<b>Proof by the Principle of Mathematical Induction</b>
WTS $\forall n \in \mathbb{Z} \geq a, P(n): 3|(2^{2n}-1)$
1. (Base Case) Show $P(1)$ is true. That is, $3|2^{2(1)}-1 \Rightarrow 2^2-1=3$ where $1 \in \mathbb{Z}$. So $3|2^{2(1)}-1$ and $P(1)$ is true.
2. (Inductive Step) $\forall n \in \mathbb{Z} \geq a, P(n) \rightarrow P(n+1) \equiv \forall n \in \mathbb{Z_n} \geq 1, 3|(2^{2n}-1) \rightarrow 3|2^{2n(n+1)}-1$.
3. Note $\forall n \in \mathbb{Z} \geq 1, 3|(2^{2n}-1) \rightarrow 3|(2^{2(n+1)}-1)$ is true by Homework 8, Problem 3.
4. By the Principle of Mathematical Induction, $\forall n \in \mathbb{Z} \geq 1, 3|2^{2n}-1$.

### Example 2
Prove that $\sum_{i=1}^{n}i=\frac{n(n+1)}{2}$.

<b>Proof by the Principle of Mathematical Induction</b>
WTS: $\forall n \in \mathbb{Z} \geq 1, P(n):\sum_{i=1}^{n}i=\frac{n(n+1)}{2}$.
1. (Base Case) WTS $P(1)$ is true.
	- LHS = $\sum_{i=1}^{n}i=\frac{n(n+1)}{2} = \sum_{i=1}^{1}i=\frac{n(n+1)}{2} = 1$
	- RHS = $\frac{n(n+1)}{2}=\frac{1(1+1)}{2}=\frac{2}{2}=1
	- The $LHS=RHS$. So $P(1)$ is true.
2. (Inductive Step) WTS: $\forall k \in \mathbb{Z} \geq 1, P(k) \rightarrow P(n+1)$
	- WTS $\forall k \in \mathbb{Z} \geq 1, \sum_{i=1}^{k}i=\frac{k(k+1)}{2} \rightarrow \sum_{i=1}^{k+1}i=\frac{(k+1)((k+1)+1)}{2}$
	- Let $k \in \mathbb{Z} \geq 1$ such that $P(k)$ is true. That is, $\sum_{i=1}^{k}i=\frac{k(k+1)}{2}$ (inductive hypothesis).	
	- WTS: $\sum_{i=1}^{k+1}i=\frac{(k+1)((k+1)+1)}{2}$
	 - $\sum_{i=1}^{k+1}i=1+2+3+4+...+k+(k+1)$
	 - $=\sum_{i=1}^{k}i + (k+1)$
	 - $=\frac{k(k+1)}{2} + (k+1)$ by the Inductive Hypothesis.
	 - $\frac{k^2+k}{2} + \frac{2(k+1)}{2}$
	 - $\frac{k^2+k+2k+2}{2}=\frac{k^2+3k+2}{2}$
	 - $=\frac{(k+1)(k+2)}{2}$
	 - $=\frac{(k+1)((k+1)+1)}{2}$
	 - So, $\sum_{i=1}^{k+1}i=\frac{(k+1)((k+1)+1)}{2}$, therefore $P(k+1)$.
	 - Therefore, by the Principle of Mathematical Induction $\sum_{i=1}^{n}i=\frac{n(n+1)}{2}$.

### Example 3
Define a sequence $b_1,b_2,b_3,...$ be letting $b_1=2$ and $b_k=\frac{b_{b-1}}{k}$ for all $k \geq 2$.
Prove that $b_n = \frac{2}{n!}$ for all $n \geq 1$.
$(b_n)_{n=1}^{\infty}=(2,\frac{2}{2},,\frac{1}{3},\frac{\frac{1}{3}}{4},...)$

<b>Proof by the Principle of Mathematical Induction</b>
WTS: $\forall n \in \mathbb{Z} \geq 1, P(n): b_n=\frac{2}{n!}$ 
1. (Base Case) WTS $P(1)$ is true.  WTS: $b_1 = \frac{2}{1!}$
	- LHS: $b_1 = 2$ by the initial condition in the sequence definition.
	- RHS: $\frac{2}{1!} = \frac{2}{1}  = 2$
	- $LHS=RHS$. So $b_1 = \frac{2}{1!}$ and $P(1)$ is true.
2. (Inductive Step) WTS: $\forall n \in \mathbb{Z} \geq 1, P(n) \rightarrow P(n+1)$
	- WTS: $\forall n \in \mathbb{Z} \geq 1, b_n=\frac{2}{n!} \rightarrow b_{n+1}=\frac{2}{(n+1)!}$
	- Let $n \in \mathbb{Z} \geq 1$ such that $P(n)$ is true.
	- That is, $b_n = \frac{2}{n!}$ (inductive hypothesis)
	- WTS: $b_{n+1} = \frac{2}{(n+1)!}$
	- Note, $b_{n+1} = \frac{b_n}{k+1}$ by the recursive formula
	- $=b_k=\frac{1}{k+1}$ by substitution.
	- $= \frac{2}{k!}*\frac{1}{k+1}$ by the inductive hypothesis.
	- $=\frac{2}{(k+1)!}$.
	- So, $b_{k+1}=\frac{2}{(k+1)!}$. Therefore, $P(k+1)$ is true.
	- Therefore, by the Principle of Mathematical Induction: $\forall n \in \mathbb{Z} \geq 1, P(n): b_n=\frac{2}{n!}$ .
	