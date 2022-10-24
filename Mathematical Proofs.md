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

### Direct Proof Form (Non-Conditional Statements)
<u>Claim:</u> $\forall x \in D, Q(x)$
<u>Proof:</u> Let $x$ be any arbitrary but particular element of D.
> The only things we know about x are things we know about every element of D.

Since $x$ is in $D$, we must have $P_1(x)$ by $J_1$
Since $P_1(x)$, we know $P_2(x)$ by $J_2$
Since $P_{n-1}(x)$, we know $P_n(x)$ by $J_n$
Since $P_{n}(x)$, we know $Q(x)$ by $J_{n+1}$

Therefore, by direct proof,
$\forall x \in D, Q(x)$

#### Basic Definitions
$\mathbb{Z} = \{\text{integers}\} = \{..., -3, -2, -1, 0, 1, 2, 3, ...\}$
$\mathbb{Q}  = \{\text{rational numbers}\} = \{\frac{a}{b} | a, b \in \mathbb(Z) \land b \neq 0\} = \{\frac{1}{2}, \frac{-3}{4}, \frac{-5286}{152}, ...\}$
$\mathbb{R} = \{\text{real numbers}\} = \{\text{all numbers on the number line}\}$
$\mathbb{R} - \mathbb{Q} = \{\text{irrational numbers}\} = \{x \in \mathbb{R} | x \notin \mathbb{Q}\}$
$\mathbb{N} = \{\text{ positive integers }\} = \{x \in \mathbb{R} | x \notin \mathbb{Q}\}$

Properties:
<u>Def:</u> $\forall n \in \mathbb{Z}, n \text{ even } \leftrightarrow [\exists k \in \mathbb{Z} | n = 2k]$
<u>Def:</u> $\forall n \in \mathbb{Z}, n \text{ odd } \leftrightarrow [\exists k \in \mathbb{Z} | n = 2k+1]$
<u>Def:</u> $\forall n \in \mathbb{Z}, n \text{ composite } \leftrightarrow [\exists a, b \in \mathbb{N} | n = a * b \land 1 < a < n]$
<u>Def:</u> $\forall n \in \mathbb{Z}, n \text{ prime } \leftrightarrow [(n > 1) \land \forall a, b \in \mathbb{N} | a * b = n \leftrightarrow (a = 1 \lor a = n)]$

---
<u>Claim:</u> $\forall n \in \{\text{evens}\}, n + 6 \text{ is even}$
<b>Proof:</b> Let $n$ be any arbitrary but particular even integer.
Then, as $n$ even, there exists an integer $k$ s.t. (such that) $n = 2k$ by definition of even.
Consider $n + 6$.
	$n + 6 = 2k + 6$ by substitution
				$= 2k + 2*3$ by observation
				$= 2(k + 3)$ by factoring 

Hence, as $k \in \mathbb{Z}$ and $3 \in \mathbb{Z}$, $k + 3 \in \mathbb{Z}$, by Closure of $\mathbb{Z}$ under $+$.
Thus, since $n + 6 = 2(k + 3)$ with $k + 3 \in \mathbb{Z}$, $n + 6$ even by definition of even.
Therefore, by direct proof, $\forall n \in \{\text{ evens}\}, n + 6$ is even.

> <b>Theorem:</b> Integers closed under $+$: $\forall n, m \in \mathbb{Z}, n + m \in \mathbb{Z}$
Integers closed under $*$: $\forall n, m \in \mathbb{Z}, n * m \in \mathbb{Z}$

### Method of Exhaustion vs Direct Proof
Method of exhaustion proves <u>each</u> thing individually, whilst direct proof proves that <u>any</u> element in $D$ will make the predicate true.

Method of exhaustion focuses on the elements whilst direct proof focuses on the properties that everything in the domain shares.

> To show anything with the property of being in $D$ has the property of making the predicate true.

### Direct Proof Form (Conditional Statements)
<u>Claim:</u> $\forall x \in D, P(x) \rightarrow Q(x)$

### Proof Facts
$\mathbb{Z}$ closed under $+$.
$\mathbb{Z}$ closed under $*$.
$\mathbb{Z}$ closed under $-$.
$\mathbb{Z}$  is not closed under $\div$.

## Direct Proof Examples
<b>Claim:</b> $n - m = 1, \text{ for any odd } m \text{ and even } m$.
<b>Logic:</b> $\forall n \in \text{\{odds\}}, \forall  m \in \text{\{evens\}}, n-m=1$
<b>Negation:</b> $\exists n \in \text{\{odds\}}, \exists m \in \text{\{evens\}}| n-m\neq1$ 
<b>Disproof:</b>
- WTS the negation, i.e. $\exists n \in \text{\{odds\}}, \exists m \in \text{\{evens\}}| n-m\neq1$.
- Let $n=5$ and $m=2$.
- Note, $n=5=2(2)+1$ with $2 \in \mathbb{Z}$, so $5$ odd by definition of odd.
- Next, $m=2=2*1$ with $1 \in \mathbb{Z}$, so $2$ even by definition of odd.
- Further, $n-m=5-2 \neq 1$.
Therefore, by example, $\exists n \in \text{\{odds\}}, \exists m \in \text{\{evens\}}| n-m\neq1$ $\exists n \in \text{\{odds\}}, \exists m \in \text{\{evens\}}| n-m\neq1$

<b>Claim:</b> $\forall n \in \mathbb{Z}, n \text{ even} \rightarrow n^2 \text{ even}$
<b>Scratchwork:</b>
$n=2k$
$n^2=(2k)^2=4k^2=2(2k^2)$
>Wait... $n$ even and $n \in \mathbb{Z}$
>	thus, by HW, $n*n$ is even.
<b>Proof:</b>
- Let $n$ be any arbitrary/particular integer.
- Assume $n$ even.
-  Note, as $n$ even and $n \in \mathbb{Z}$, $n^2 = n*n$ is even, by homework.
Therefore, by direct proof, $\forall n \in \mathbb{Z}, n \text{ even} \rightarrow n^2 \text{ even}$.

> <b>Fact:</b> $\forall n \in \mathbb{Z}, n \text{ odd } \rightarrow n^2 \text{ odd }$.

<b>Claim:</b> $\forall n \in \mathbb{Z}, n^2-n \text{ even }$
<b>Proof:</b>
- Let $n$ be any arbitrary/particular integer.
- Note, $n$ can be even or odd.
- Proceed by division into cases.
	- <u>Case 1:</u> $n$ even
	- Since $n$ even, $n=2k$ for some $k \in \mathbb{Z}$, by definition of even.
	- Consider $n^2-n=(2k)^2-2k$ by substitution.
	- $n^2-n=4k^2-2k$ by simplificiation.
	- $n^2-n=2(2k^2-k)$ by factoring.
	- Note, as $2, k \in \mathbb{Z}$, $2k^2-k \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $*$ and $-$.
	- Hence, as $n^2-n=2(2k^2-k)$ with $2k^2-k \in \mathbb{Z}$, $n^2-n$ even, by definition of even.
	
	- <u>Case 2:</u> $n$ odd 
	- Since $n$ even, $n=2t+1$ for some $t \in \mathbb{Z}$, by definition of odd.
	- Consider $n^2-n$, note $n^2-n=(2t+1)^2-(2t+1)$ by substitution
	- $n^2-n=(2t)^2+2t+2t+1-(2t+1)$ by distribution
	- $n^2-n=4t^2+4t+1-2t-1$ by simplification
	- $n^2-n=4t^2+2t$ by simplification
	- $n^2-n=2(2t^2+t)$ by factoring
	- Note, as $2, t \in \mathbb{Z}$, $2t^2+t \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $*$ and $+$.
	- Hence, as $n^2-n=2(2t^2+t)$ with $2t^2+t \in \mathbb{Z}$, $n^2-n$ even by definition of even.
- Thus, by division into cases, $n^2-n$ even in general.
Therefore, by direct proof $\forall n \in \mathbb{Z}, n^2-n \text{ even }$.

>Any time you can separate the domain into categories which together cover the problem domain, you can break these categories into cases and prove the claim for each category separately as shown above.

<b>Claim:</b> For any 3-digit number, if the sum of the digits is divisible by $3$, then the number itself is also divisible by $3$.
<b>Logic:</b> $\forall a_{100},a_{10},a_1 \in \{0,...,9\}, 3|a_{100}+a_{10}+a+1 \rightarrow 3|100*a_{100}+10*a_{10}+1*a_1$
<b>Scratchwork:</b> How to rewrite the then-part in terms of the if-part?
$100a_{100}+10a_{10}+1a_1=99a_{100}+9a_{10}+(a_{100}+a_{10}+a_1)$
Assuming, $3|(a_{100}+a_{10}+a_1)$

<b>Proof:</b>
- Let $a_{100},a_{10},a_1$ be arbitrary/particular numbers in $\{0,1,...,9\}$.
- Assume $3|(a_{100} + a_{10} + a_1)$.
- Consider $a_{100} + a_{10} + a_1$. WTS $3|(100a_{100} + 10a_{10} + a_1)$. 
- Note, $100a_{100} + 10a_{10} + a_1 = (99+1)a_{100} + a_{10} + a_1$ by evaluation.
- $= 99a_{100}+a_{100}+9a_{10}+a_{10}+a_1$ by substitution.
- $= 99a_{100}+9a_{10}+(a_{100}+a_{10}+a_1)$, by commutativity of addition.
- WTS $99a_{100}$ and $9a_{10}$ are multiples of $3$.
- Note, as $9 = 3*3$ with $3 \in \mathbb{Z}$, $3|9$ by defintion of divides.
- Further, as $3|9$, $3|9a_{10}$ by fact from class.
- Next, as $99 = 3*33$, with $33 \in \mathbb{Z}$, $3|99$ by defintion of divides.
- Again, as $3|99$, $3|99a_{100}$ by fact from class.
- Thus, since $3|99a_{100}$ and $3|9a_{10}$ and $3|(a_{100}+a_{10}+a_1)$, $3|(99a_{100}+9a_{10}+(a_{100}+a_{10}+a_1)) = 100a_{100}+10a_{10}+a_1$, by fact from class.
- Therefore, by direct proof: $\forall a_{100},a_{10},a_1 \in \{0,...,9\}, 3|a_{100}+a_{10}+a+1 \rightarrow 3|100*a_{100}+10*a_{10}+1*a_1$