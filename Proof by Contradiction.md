Form of [[Indirect Proof]]

> Contradiction is the old lawyer catching a witness in a lie trick.  You start by assuming what you're trying to prove true is false, and then see where that logically leads, hoping it leads to something obviously false/contradictory. (Like someone being in two places at once or $1 = 0$)

<b>Idea 1:</b> If from $A$ we can dedcue a fake statement, then $A$ is false as well.
<b>Idea 2:</b> To prove a statement $S$ true, try to show its opposite $\sim S$ is false.  Do this by assuming $\sim S$ is true and deducing something fake from that.  If $\sim S$ is false, thast means $S$ is also false.

<b>Claim:</b> No integer can be both even and odd.
<b>Logic:</b>  $\forall n \in \mathbb{Z}, \sim (n \text{ even } \land \text{ odd })$
<b>Negation:</b>  $\exists n \in \mathbb{Z} | n \text{ even } \land n \text{ odd}$
<b>Proof:</b>  Proof by contradiction.  Suppose for sake of contradiction, the negation is true. i.e: $\exists n \in \mathbb{Z} | n \text{ even } \land n \text{ odd}$.
- Since $n$ even, $n = 2k$$ for some $k \in \mathbb{Z}$ by definition.
- Since $n$ odd, $n = 2j + 1$$ for some $j \in \mathbb{Z}$ by definition.
- Consider, $n = 2k$. If $n = 2k \Rightarrow, 2k = 2j +1$ by substitution.
- $1 = 2k -2j$ by subtracting $2j$ from both sides.
- $1 = 2(k-j)$ by factoring.
- $\frac{1}{2} = k-j$ by dividing both sides by $2$.
- Note, as $k, l \in \mathbb{Z}$ , $k-l \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under subtraction.
- Thus, $\frac{1}{2} = k-j \in \mathbb{Z}$. ($\rightarrow \leftarrow$).
- Contradiction! $\frac{1}{2} \notin \mathbb{Z}$. Thus, our assumption of the negation is false so the original statement is true by definition.

<b>Logic:</b>  $\forall p \in \mathbb{N}, \forall a \in \mathbb{N}, \forall c \in \mathbb{N}, p|a \land c<p \rightarrow p \nmid (a + c)$
<b>Negation:</b>  $\exists p \in \mathbb{N} | \exists a \in \mathbb{N} | \exists c \in \mathbb{N} | p|a \land n < p \land p | (a+c)$
<b>Proof:</b>  Proof by contradiction.  Suppose for sake of contradiction, the negation is true. i.e: $\exists p \in \mathbb{N} | \exists a \in \mathbb{N} | \exists c \in \mathbb{N} | p|a \land n < p \land p | (a+c)$.
- Note, as $p|a$, $a=pk$ for some $k \in \mathbb{Z}$.
- Further, as $p|(a+c)$, $a+c = pl$ for some $l \in \mathbb{Z}$.
- Consider $a+c=pl$. Note,
- $a+c=pl$ by above.
- $pk+c=pl$ by the above.
- $c=pl-pk$ by subtracting from both sides.
- $c=p(l-k)$ by factoring.
- Note, as $l,k \in \mathbb{Z}$, $l-k \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under subtraction.
- Thus, since $c=p(l-k)$ with $l-k \in \mathbb{Z}$, $p|c$ by definition.
- However, since $c < p$, $p \nmid c$ by Question 1 on WA 9.
- ($\rightarrow \leftarrow$) Contradiction!  We can't have both $p|c$ and $p \nmid c$, thus negation is false, so original is true by contradiction.

<b>Claim:</b> $\forall x \in \mathbb{R*}, x \in \mathbb{Q} \rightarrow \pi*x \notin \mathbb{Q}$
<b>Proof:</b> Proof by contrapositive. Note the contrapositive is: $\forall x \in \mathbb{R*}, \pi*x \in \mathbb{Q} \rightarrow x \notin \mathbb{Q}$.