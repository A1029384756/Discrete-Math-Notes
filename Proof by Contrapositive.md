Form of [[Indirect Proof]]

<b>Claim:</b> $\forall x \in \mathbb{D}, P(x) \rightarrow Q(x)$
<b>Proof:</b> Proof by contrapositive. Note the contrapositive is: $\forall x \in \mathbb{D}, \sim Q(x) \rightarrow \sim P(x)$.
Prove the contrapositive by any means.
Thus, by contrapositive, $\forall x \in \mathbb{D}, P(x) \rightarrow Q(x)$.

> Contrapositive proof form only works on [[Conditional Statements]].

<b>Claim:</b> $\forall y \in \mathbb{Q}, x \in \mathbb{R}\backslash\mathbb{Q} \rightarrow x + y \in \mathbb{R}\backslash\mathbb{Q}$
>$\mathbb{R}\backslash\mathbb{Q}$: Set of all irrational numbers.

<b>Proof:</b> Proof by contrapositive. Note the contrapositive is: $\forall x \in \mathbb{R}, \forall y \in \mathbb{Q}, x+y \in \mathbb{Q} \rightarrow x \in \mathbb{Q}$.
- Let $x$ be any arbitrary/particular real number and let $y$ be any arbitrary/particular rational number.
- Assume $x+y \in \mathbb{Q}$.
- Consider, $x$. WTS $x \in \mathbb{Q}$.
- Note $x=(x+y)-y$, by simplification.
- Thus, as $x+y, y \in \mathbb{Q}$, $x=(x+y)-y\in \mathbb{Q}$, by closure of $\mathbb{Q}$ under subtraction.
- Therefore, by direct proof $\forall x \in \mathbb{R}, \forall y \in \mathbb{Q}, x+y \in \mathbb{Q} \rightarrow x \in \mathbb{Q}$.
- Thus, by contrapositive, $\forall y \in \mathbb{Q}, x \in \mathbb{R}\backslash\mathbb{Q} \rightarrow x + y \in \mathbb{R}\backslash\mathbb{Q}$.

> Indirect proof is useful when the things that are being studied are difficult to write in a manner that is useful for proofs.  This includes:
> - Square roots
> - Things defined in terms of what they are not rather than what they are (irrational numbers, primes, not-divides, not equals, etc.)

<b>Claim:</b> $\forall x \in \mathbb{R}, x \in \mathbb{Q} \rightarrow \pi*x \notin \mathbb{Q}$
> <b>Fact:</b> $\pi \in \mathbb{R}\backslash\mathbb{Q}$

<b>Disproof:</b> Note the negation is: $\exists x \in \mathbb{R} | x \in \mathbb{Q} \land \pi*x \in \mathbb{Q}$.
- Let $x = 0$.
- Note $0 = \frac{0}{1}$, so $0 \in \mathbb{Q}$, as required.
- Further, $0*\pi = 0 \in \mathbb{Q}$, as desired.
- Hence, by example, $\exists x \in \mathbb{R} | x \in \mathbb{Q} \land \pi*x \in \mathbb{Q}$.
- Thus, the negation is true, so the claim is false.

