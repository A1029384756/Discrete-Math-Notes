A <u>set</u> is a collection of elements such that everything in the universe is either in $\in$ or out $\notin$ of the set.

The only way in which an element can relate to a set is by being in or out.

<b>Arrays:</b>
- Have order and multiplicity

<b>Bags:</b>
- Have multiplicity but no order

<b>Sets:</b>
- Don't have order or multiplicity

Sets can exist within other sets [[Subsets]].

> An element and the set containing that element are <b>DIFFERENT THINGS</b>.
	$\pi \neq \{\pi\}$
	$\pi \notin \{\{\pi\}\}$


<b>Example:</b>
$A = \{a,b,c\}$
$S = \{A, (1,0,0,1), a, b, \{c\}\}$

$a \in S$
$b \in S$
$c \notin S$
$\{a\}\notin S$
$\{b\}\notin S$
$\{c\}\in S$
$\{a,b\}\notin S$
$\{a,b,c\}\in S$

---

### Set Builder Notation 
A way to express sets with infinitely many elements.

$\{x \in \mathbb{D} | P(x)\}$
$x \in \mathbb{D}$ $\rightarrow$ form of elements in the set
$P(x)$ $\rightarrow$ property elements in our set must have 
$\{exp(x) | P(x)\} \rightarrow$ set of all elements with form $exp(x)$ such that $x$ has property $P$
$3\mathbb{Z} = \{3k|k \in \mathbb{Z}\} = \{...,-6,-3,0,3,6,...\}$

<b>Claim:</b> $2\mathbb{Z} \cap 3\mathbb{Z} = 6\mathbb{Z}$

### Set Equality
We say two sets are equal if they have the same elements. _Does not necessarily mean they have the same size._

## Proving Subsets if Sets are Infinite
**Claim:** $\mathbb{Z} \subseteq \mathbb{Q}$
**Proof:** WTS $\forall n \in \mathbb{Z}, n \in \mathbb{Q}$
Let $n$ be any arb/part integer.
Note, $n = \frac{n}{1}$ by simplification.
This, as $n = \frac{n}{1}$ with $n,1 \in \mathbb{Z}$ and $1 \neq 0$, $n \in \mathbb{Q}$, by def of $\mathbb{Q}$.
Therefore, by element method of proof, $\mathbb{Z} \subseteq \mathbb{Q}$.

**Element Method of Proof** is proving $A \subseteq B$ by starting with an arb/part $x \in A$ and showing that is must also be in $B$.

**Claim:** $6 \mathbb{Z} \subseteq 3\mathbb{Z}$
**Proof:** WTS $\forall n \in 6\mathbb{Z}, n \in 3\mathbb{Z}$
Let $n$ be any arb/part integer in $\mathbb{6Z}$
Since $n \in 6\mathbb{Z}$, $n=6k$ for some $k \in \mathbb{Z}$
WTS $n = 3t$ for some $t \in \mathbb{Z}$
Note, $n = 6k$, by the above
$n = (3*2)k$ by evaluation
$n=3(2k)$ by associativity
Note, as $2,k \in \mathbb{Z}$, $2k\in\mathbb{Z}$ by closure of $\mathbb{Z}$ under mult.
Thus, as $n = 3(2k)$, with $2k\in\mathbb{Z}$, $n\in3\mathbb{Z}$ by definition of $3\mathbb{Z}$
Therefore, by element method, $6 \mathbb{Z} \subseteq 3\mathbb{Z}$

### Additional Definitions
$\varnothing = \{\} \leftarrow$ Empty Set
$P(A) = \{B | B \subseteq A\} \leftarrow$ Power set, set of all subsets of $A$

We say $\varnothing \subseteq A$ for any set $A$.