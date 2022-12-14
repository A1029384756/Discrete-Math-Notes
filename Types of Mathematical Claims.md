1. <b>Unproven</b>
	- Conjecture
		 - Collatz Conjecture
		 - Twin Prime Conjecture
1. <b>Proven</b>
	- <u>Proposition</u> - A small fact following directly from a definition.
	- <u>Lemma</u> - A small fact which helps prove a bigger more important fact.
	- <u>Theorems</u> - Big important facts.
	- <u>Corollary</u> - Smallish fact that follows directly from a theorem.

> <b>Definition:</b> $\mathbb{Q} = \{\frac{a}{b} | a,b \in \mathbb{Z} \text{ with } b \neq 0\}$

> <b>Proposition:</b> Every rational $x$ can be written as $\frac{a}{b}$ in simplified form. (i.e., $a$ and $b$ share no nontrivial factors).  Clearly then, a fraction in simplied form cannot have the numerator and denominator both be even.

><b>Lemma:</b> $\forall n \in \mathbb{Z}, n^2 \text{ even } \rightarrow n \text{ even}$

> <b>Theorem:</b> $\sqrt{2}$ is irrational.

<b>Negation:</b> $\sqrt{2}$ is rational.
<b>Proof:</b> Assume for the sake of contradiction that $\sqrt{2}$ is rational.
- Since $\sqrt{2}$ rational, $\sqrt{2} = \frac{a}{b}$ in simplified form by proposition.
- Note, importantly, this means $a$ and $b$ share no factors, in particular, they cannot both be even.
- Consider $\sqrt{2} = \frac{a}{b}$, Note
	- $\sqrt{2} = \frac{a}{b}$
	- $2 = \frac{a^2}{b^2}$
	- $2b^2 = a^2$
	- Since $b \in \mathbb{Z}, b^2 \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under multiplication.
	- Then, as $a^2=2b^2$, with $b^2 \in \mathbb{Z}, a^2$ even.
	- Then, since $a^2$ is even, $a$ must be even by the above lemma.
	- As $a$ even, $a=2k$ for some $k \in \mathbb{Z}$ by definition of even.
	- Thus, $2b^2=a^2 \Rightarrow 2b^2 = (2k)^2 \Rightarrow 2b^2=4k^2 \Rightarrow b^2 = 2k^2$ 
	- Since $k \in \mathbb{Z}$, $k^2 \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under multiplication.
	- As $b^2 = 2k^2$ with $k^2 \in \mathbb{Z}$, $b^2$ is even by definition.
	- Then, since $b^2$ even, $b$ even by lemma. ($\rightarrow \leftarrow$)
	- Contradiction! Since $\frac{a}{b}$ is simplified form, $a$ and $b$ cannot both be even. Thus, the negation is false and as such, $\sqrt{2}$ is irrational.

### Chicken McNugget Problem
<b>Set-Up:</b> McDonald's sells McNuggets in 4pc and 5pc packs.
<b>Claim:</b> $\forall n \in \mathbb{Z}_{\geq 12}$, we can buy exactly $n$ nuggets from McDonald's.
<b>Proof:</b> Proof by Strong Induction
- <u>Base Cases</u>
	- Let $n = 12$. Note $12 = 3*4$
	- Let $n = 13$. Note $13 = 2*4 + 5*1$
	- Let $n = 14$. Note $14 = 1*4 + 5*2$
	- Let $n = 15$. Note $15 = 3*5$
- <u>Inductive Step:</u>
	- WTS $\forall n \geq 15, P(12) \land P(13) \land ... \land P(n) \rightarrow P(n+1)$
	- Let $n$ be any arbitrary/particular integer greater than $15$.
	- Assume $12$ through $n$ can all be made with $4pc$ and $5pc$.
	- Consider $(n+1) -4 = n-3$.
	- Since $n \geq 15$, $n-3 \geq 12$, thus, $n-3$ can be made with $4pc$ and $5pc$ packs, ie. $n-3=4k+5l$.
	- Then, $n+1=(n-3)+4 = 4k+5l+4=4(k+1)+5l$.
	- Hence, $n+1$ can be made with $4pc$ and $5pc$ packs.