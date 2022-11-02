
> Maybe: $\text{"From a we deduce B" is valid if } A \rightarrow B \equiv T \text{ and invalid if } A \rightarrow B \equiv F$
> Problem: $\text{Burt is a mammal} \rightarrow \text{ Burt is a cat} \equiv T \rightarrow T \equiv T$. But it is not true that Burt is a mammal $\Rightarrow$ Burt is a cat

The issue is that <b>if-then</b> ([[Logical Operations]]) [[Statement|Statements]] alone are prone to coincidences.  Just because $p \rightarrow q \equiv T$ does not mean that anything with the form of p wil lead to something with the form of q.

---

# Predicates
<b>Def:</b> A predicate is a sentence with a variable which becomes a [[Statement]] when something from its domain (set of acceptable inputs) is plugged in for the variable.

Ex: $P(x) \equiv x$ is bald, with domain $D = { \text{set of all people} }$
Ex: $Q(a) \equiv \text{a is a cat}$, with domain $E = \text{set of all animals}$
Ex. $R(s) \equiv s$ is attending class today, with domain $S = \text{set of all students}$
Ex. $T(y) \equiv (y^2 = 2)$ with domain $\mathbb{R} = \text{set of real numbers}$

<b>Def:</b> The <u>truth set</u> of predicate $P(x)$ with domain $D$ is the set of a
ll things in $D$ which when plugged into $P(x)$ output a true [[Statement]].

Ex: $M(y) \equiv (y^2 = 4)$ with domain $\mathbb{R} = \text{set of real numbers}$. The truth set of $M = \{2, -2\}$

>How can we make a predicate $P(x)$ with domain $D$ into a [[Statement]]?

1. Plug something from the domain in!
	1. $P(x) \equiv x$ is a cat with domain $D = \{animals\}$
	2. $P(\text{louie})$ is a [[Statement]]
	3. $P(\text{Valvo})$ is also a [[Statement]]
2. Quantify on what range you are claiming the predicate to be true.
	1. For all $x$ in $\{\text{animals}\}$, $P(x)$ $\rightarrow$ Range we're claiming predicate works on.
	2. There exists an $x$ in $\{\text{animals}\}$ such  that $P(x)$ is true.

# Quantifiers
### Universal Quantifier
$\forall$ - "For all", "For every", "For each", "For any"
Used to make <u>universal [[Statement]]s</u>

>Can use to make <u>universal [[Statement]]s</u>, which is any [[Statement]] of the form, $\forall x \in D, P(x)$

Ex. | 
	(a) $\forall p \in \{ \text{people in this class}\}$, p likes math $\equiv T$
	(b) $\forall p \in \{\text{pople in this class}\}$, p goes to VT. $\equiv T$
	(c) Each Formula 1 team has 2 drivers. $\equiv \forall t \in \{\text{Formula 1 teams}\}$, $Q(t)$ where $Q(t) \equiv t$ has 2 drivers
	(d) For any pen in my bag, it is clickable -> $\forall x \in \{\text{Pens in my bag}\}$, x is clickable 

### How to Prove a Universal [[Statement]] is True:
<u>Claim:</u> (d)
<u>Proof:</u> Consider a pen $x \in \{\text{black pen, blue pen, red pen, purple pen}\}$.  Proceed by dividing into cases.
	<u>Case 1:</u> $x$ is the black pen. -> WTS: $x$ is clickable.  Not the black pen is clickable by observation.
	<u>Case 2:</u> $x$ is the blue pen. -> WTS: $x$ is clickable.  Not the blue pen is clickable by observation.
	<u>Case 3:</u> $x$ is the red pen. -> WTS: $x$ is clickable.  Not the red pen is clickable by observation.
	<u>Case 4:</u> $x$ is the purple pen. -> WTS: $x$ is clickable.  Not the purple pen is clickable by observation.

Thus, by the method of exhaustion, $\forall x \in \{\text{pens in my bag}\}$, x is clickable.

### Universal Conditional [[Statement]]
- Any [[Quantifiers#Universal Quantifier | Universal Statement]] where the predicate is an [[Logical Operations#^600c2f |if-then]], int he form $\forall x \in D, P(x) \rightarrow Q(x)$

(e) $\forall p \in \{\text{people on Earth}\}$, p in the class $\rightarrow$ p goes to VT.
(f) For any animal, if it's a cat, then it's a mammall $\equiv \forall a \in \{\text{animals}\}$, a is a cat $\rightarrow$ a is a mammal.
(g) For any animal, if it's a mammal then it's a cat.

---

Are (b) and (e) saying different things?
>No they're the same!

>IDEA: Notice the domain and the if-part both work to restrict which things we're talking about.

Ex.| $\forall a \in \{\text{animals}\}$, a is a cat $\rightarrow$ a is a mammal $\equiv \forall a \in \{\text{cats}\}$, a is a mammal.
Ex.| $\forall t \in \{\text{F1 teams}\}$, t has 2 drivers $\equiv \forall$ .

### Existential Quantifier:
$\exists$ - means "there exists", "there is some", "for one", "for some".
> We use $\exists$ to create <u>existential statements</i> which are of the form $\exists x \in D | P(x)$ 

$\exists!$ - means "there exists exactly one"
> This is used to specify when existence is limited to one item

Ex. |
	(h) Some person in this class is from NOVA. $\equiv \exists p \in \{\text{this class}\} | x \text{ is from NOVA}$
	(i) There exists a number is when squared is 64. $\equiv \exists p \in z | n^2 = 64$
	(j) For one person on Earth, they are Valvo's mother. $\equiv \exists y \in \{\text{people on Earth}\}$, y is Valvo's mother.

<u>Claim:</u> (h)
<u>Proof:</u> Let $p \equiv \text{Adrian}$.

- Note Adrian is in this class.
- Futher Adrian is from NOVA.
- Thus, by example, $\exists p \in \{\text{this class}\} | p$ is from NOVA.

### How to Negate $\forall$ and $\exists$ Statements
>The opposite of $P(x)$ being true for all $x \in D$ is $P(x)$ is true for some $x \in D$

>$\sim (\forall x \in D, P(x)) \equiv \exists x \in D | \sim P(x)$.
>$\sim (\exists x \in D | P(x)) \equiv \forall x \in D, \sim P(x)$.

How to disprove $\forall$ and $\exists$ statements:
	We disprove a statement (i.e. prove it false) by proving it's negation true.

Ex. |
	<u>Claim:</u> $\exists p \in \{\text{the class}\}$, p is from New Jersey.
	<u>Disproof:</u> Need to show the negation, $\forall o \in \{\text{the class}\}$, p is not from New Jersey.

$\forall x \in \{2, 3, 78\}$, $x^2 > x$ $\equiv$ $2^2>2 \land 3^3>3 \land 78^2>78$ 
> In general, $\forall x \in \{d_1, d_2, ... d_n\}, P(x) \equiv P(d_1) \land P(d_2) \land P(...) \land P(d_n)$
> $\exists x \in \{d_1,d_2,...d_n\} | P(x) \equiv P(d_1) \lor P(d_2) \lor P(...) \lor P(d_n)$
> $\exists! x \in \{d_1, d_2, ..., d_n\} | P(x) \equiv P(d_1) \oplus P(d_2) \oplus P(...) \oplus P(d_n)$

> These are literally $\land, \lor, \text{and} \oplus$ statements only as long as the domain is finite.
> With this idea, $\sim(\forall x \in \{d_1, d_2, ..., d_n\}) \equiv \sim(P(d_1) \land P(d_2) \land ... P(d_n)) \\ \equiv \sim P(d_1) \lor P(d_2) \lor P(d_n) \equiv \exists x \in \{d_1, d_2, ... d_n\} | \sim P(x)$

The way to prove a [[Statement]] false is to disprove it.
Disproving a [[Statement]] means to prove it's negation true.

Every quantified statement has <u>one</u> quantifier and <u>one</u> predicate BUT statements can appear to have multiple quantifiers because predicates are complex.

Ex. |
$\forall t \in \{\text{Packers, Patriots, Chiefs}\}, \exists p \in \{\text{NFL Players}\} \text{ p is the qb for t}$
For all t in {Packers, Patriots, Chiefs}, Q(t).

<u>Proof:</u> Let t be in {Packers, Patriots, Chiefs}
Proceed by division into cases.
<u>Case 1:</u> t = Packers
<u>Case 2:</u> t = Patriots 
<u>Case 3:</u> t = Chiefs 