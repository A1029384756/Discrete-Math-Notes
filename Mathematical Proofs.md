<b>Definition:</b> A <u>mathematical proof</u> is a sequence of statements (the body of the proof) leading to a <u>conclusion</u>.

<b>Definition:</b> A <u>proof form</u> is <u>valid</u> if in every situation where the body is true, the conclusion is true also.

<b>Definition:</b> A proof is <u>valid</u> if it's form is valid and each statement of the body is true.

>The conclusion of a sound proof must be true.

Ex. |
<b>Method of Exhaustion Form</b>
Claim: $\forall x \in \{D_1, D_2,..., D_n\}, P(x)$
Proof: Let $x$ be in $D$

<b>Case 1:</b> $x = D_1$, Show $P(D_1)$
<b>Case 2:</b> $x = D_2$, Show $P(D_2)$
<b>Case 3:</b> $x = D_2$, Show $P(D_2)$

Therefore, by method of exhaustion, $\forall x \in \{D_1, D_2,..., D_n\}, P(x)$.

Ex. |
<b>Proof by Example Form</b>
Claim: $\exists x \in D | P(x)$
Proof: Let $x = D$
Note $d \in D$ as required
Further, show $P(d)$ is true

Therefore, by example, $\exists x \in D | P(x)$.

Remember that a [[Knowing what is True#Deduction | Deduction]] is valid as long as the criteria $\forall x \in D, A(x) \rightarrow B(x) \equiv T$.

<u>How do we use deductions?</u> 
> Remember that the point of a deduction is to use the truth of A(d) to determine the truth of B(d).

Suppose we know: (1) $\forall x \in D, A(x) \rightarrow B(x) \equiv T$  AND (2) $A(d) \equiv T$.

Then since $A(d) \equiv T$ and $\forall x \in D, A(x) \rightarrow B(x) \equiv T$, we must have $B(d) \equiv T$ as well!

---
We write this by saying:
"From $A(d)$, we can deduce $B(d)$ by J." (J meaning justification and is a [[Statement]])
"SInce $A(d)$, we know $B(d)$ by J."
"As $A(d)$, we get $B(d)$ by J."
"Then, $A(d)$, by$B(d)$ and J."
> All of these expressions are saying the same thing.

---
Ex. |
Def. | $\forall x \in \{\text{animals}\}, (\text{x is warm-blooded}) \land (\text{x has fur}) \rightarrow \text{x is a mammal}$ (Mammal Definition)

As Louie is warm-blooded $\land$ Louie has fur, we know that Louie is a mammal by Mammal Defininition.

Since Jeff the sea monkey is warm blooded $\land$ Jeff has fur, Jeff must be a mammal by the Mammal Definiition.

# Forms of Mathematical Proof
- [[Direct Proof]]
- [[Indirect Proof]]

