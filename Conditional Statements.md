### Conditional Statements
Compound statements containing $\text{"} \rightarrow \text{"}$ ^d2f73f

[[Logical Operations#^600c2f]]

$\text{"} p \rightarrow q \text{", "if p then q" or "q follows from p."}$

Ex. |
- $\text{Louie is a cat} \rightarrow \text{Louie is a mammal} \equiv T \rightarrow T \equiv T$
- $\text{Denver (Sydney's dog) is a mammal} \rightarrow \text{Denver is a cat} \equiv T \rightarrow T \equiv F$
- $\text{VT beat ODU in football} \rightarrow \text{Valvo will make it rain starburst in class} \equiv F \rightarrow F \equiv T$
- $\text{7 is even} \rightarrow \text{Valvo gave Sherman a high five at 4:10PM} \equiv F \rightarrow T \equiv T$

> $p \rightarrow q \equiv T \text{does NOT necessarily mean p is true}$
> $p \rightarrow q \equiv T \text{does NOT necessarily mean q is true}$
> $p \rightarrow q \equiv T \text{means that the connection between p and q holds}$
> <b>Connection is:</b> $\textbf{IF } \text{p is true } \textbf{THEN } \text{q must also be true}$

### Related Conditionals
- Consider the conditional statement $p \rightarrow q$
- Converse of $p \rightarrow q$ : $q \rightarrow p$
- Inverse of $p \rightarrow q$ : $\sim p \rightarrow \sim q$
- Contrapositive of $p \rightarrow q$ : $\sim q \rightarrow \sim p$

Ex. |
A. $\text{Louie is a cat} \rightarrow \text{Louie is a mammal} \equiv T$
<u>Converse of A.</u>: $\text{Louie is a mammal} \rightarrow \text{Louie is a cat} \equiv T$
<u>Inverse of A:</u> $\text{Lousie is not a cat} \rightarrow \text{Louie is not a mammal} \equiv T$
<u>Contrapositive of A:</u> $\text{Louie is not a mammal} \rightarrow \text{Louie is not a cat} \equiv T$

>Which of these is <u>saying the same thing</u> as A? (Contrapositive)
><b>Recall:</b>
>	Two expressions are saying the same thing not if they just coincidentally have the same truth value but if as expressions, their forms are equivalent.

^9b0b4f

Ex. |
- I want a burger and fries or a burger and tots.
- I want a burger and fries or tots.

Burger = p, Fries = q, Tots = r

Forms:
- $(p\land q) \lor (p \land r)$
- $p\land (q\lor r)$
Since their forms are equivalent by the distributive law, they are saying the same thing.

---

### Show Contrapositive is Saying the Same Thing as the Original
Need to show the forms are equivalent, i.e.,
	$p \rightarrow q \equiv \sim q \rightarrow \sim p$

Option A: <b>Truth Tables</b>

|$p$|$q$|$\sim p$|$\sim q$|$p \rightarrow q$|$\sim q \rightarrow \sim p$|
|---|---|---|---|---|---|
|T|T|F|F|T|$F \rightarrow F \equiv T$|
|T|F|F|T|F|$F \rightarrow T \equiv F$|
|F|T|T|F|T|$F \rightarrow T \equiv T$|
|F|F|T|T|T|$T \rightarrow T \equiv T$|

>Since every input leads to the same output, $p \rightarrow q \equiv \sim q \rightarrow \sim p$

Option B: <b>Prove Using a Chain of Logical Laws</b>
First need to learn how to write $p \rightarrow q$ in terms of $\land \lor \sim$
<u>Claim:</u>
	$p \rightarrow q \equiv \sim p \lor q$
<u>Proof:</u>

|$p$|$q$|$\sim p$|$\sim p \lor q$|$p \rightarrow q$|
|---|---|---|---|---|
|T|T|F|T|T|
|T|F|F|F|F|
|F|T|T|T|T|
|F|F|T|T|T|

>Since every output leads to the same output: $p \rightarrow q \equiv \sim p \lor q$

Negation of $p \rightarrow q$   is NOT its converse
								is NOT its inverse
								is NOT a conditional statement at all

Claim: $\sim (p \rightarrow q) \equiv p \land \sim q$
Proof: Let p and q be statements. Then:
	$\sim (p \rightarrow q) \equiv \sim (\sim p \lor q) \text{ by conditional equivalence}$
	$\equiv \sim (\sim p) \land \sim q \text{ by DeMorgan's law}$
	$\equiv p \land \sim q \text{ by double negative law}$
Therefore, by the transitive law, $\sim (p \rightarrow q) \equiv p \land \sim q$

### Biconditional Statements
IF-AND-ONLY-IF (p,q) {

|$p$|$q$|$p \leftrightarrow q$|
|---|---|---|
|T|T|T|
|T|F|F|
|F|T|F|
|F|F|T|

}

$(p \leftrightarrow q) \equiv (p \rightarrow q) \land (q \rightarrow p)$ <-- Used when doing chain of laws

$p \rightarrow q \equiv \sim q \rightarrow \sim p$
$\text{Original} \equiv \text{Contrapositive}$

$q \rightarrow p \equiv \sim p \rightarrow \sim q$
$\text{Converse} \equiv \text{Inverse}$

$p \rightarrow q \neq q \rightarrow p$
$\text{Original} \neq \text{Converse}$ <-- They can sometimes yield the same results but they say different things.
