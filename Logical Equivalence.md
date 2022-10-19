Sometimes, different looking expressions are actually the same [[Expression Identities]]] For <i>any</i> input possible, the output expressions are equivalent.  This is logical equivalence.
- ~(p$\land$q)$\equiv$~p$\lor$~q


![[Table_of_Logical_Equivalences.pdf]]

Ex. | For any statement p, q

- p$\land$q $\equiv$q$\land$p
- p$\lor$q$\equiv$q$\lor$p
- p->q$\neq$q->p

Ex. | p$\oplus$q $\equiv$ $(\sim p\land q)\lor(p\land \sim q)$

Proof:

|p|q|$\sim p$|$\sim q$|$\sim p \land q$|$p\land \sim q$|$(\sim p \land q)\lor(p \land \sim q)$|$p \oplus q$|
|---|---|---|---|---|---|---|---|
|T|T|F|F|F|F|F|F|
|T|F|F|T|F|T|T|T|
|F|T|T|F|T|F|T|T|
|F|F|T|T|F|F|F|F|
$\text{Since for every input, } p \oplus q \text{ and } (\sim p \land q)\lor(p \land \sim q) \text{ give the same outputs, } p \text{ and } q \text{ are logically equivalent.}$
Ex. | $p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$

|$p$|$q$|$r$|$p \land (q \lor r)$|$(p \land q) \lor (p \land r)$|
|---|---|----|---|---|
|T|T|T|T|T|
|T|T|F|T|T|
|T|F|T|T|T|
|T|F|F|F|F|
|F|T|T|F|F|
|F|T|F|F|F|
|F|F|T|F|F|
|F|F|F|F|F|
$\text{Since for every input they give the same outputs, } p \land (q \lor r) \text{ and } (p \land q) \lor (p \land r) \text{ are logically equivalent.}$

---
Ex. | $\sim (\text{VT is in Kansas} \land \text{VT accessible by HB}) \neq \sim \text{VT in Kansas} \land \sim \text{VT accessible by HB}$

|$p$|$q$|$\sim (p \land q)$|$\sim p \land \sim q$|
|---|---|---|---|
|T|T|F|F|
|T|F|T|F|
|F|T|T|F|
|F|F|T|T|

Ex.| $\sim (p \land q \land r) \equiv \sim p \lor \sim q \lor \sim r$
Proof:
$\text{Let p, q, and r be any statements.}$
$\sim (p \land q \land r) \equiv \sim ((p \land q) \land r) \equiv \sim (p \land q) \lor \sim r \equiv \sim p \lor \sim q \lor \sim r$

This works because of the transitive law which says: for any statements A, B, and C,
	$\text{If } A \equiv B \text{ and } B \equiv C \text{, then } A \equiv C$

---
Proof:
	$\text{Let p, q, and r be any statements. Then,}$
	$\sim (p \land q \land r) \equiv \sim ((p \land q) \land r) \rightarrow \text{ by associative law}$
		$\equiv \sim (q \land q) \lor \sim r \rightarrow \text{ by DeMorgan's law}$
		$\equiv (\sim p \lor \sim q) \lor \sim r \rightarrow \text{ by DeMorgan's law}$
		$\equiv \sim p \lor \sim q \lor \sim r \rightarrow \text{ by associative law}$
	$\text{Thus, by the transitive law,}$
		$\sim (p \land q \land r) \equiv \sim p \lor \sim q \lor \sim r$


Ex. |

Claim: $(p \land q) \oplus p \equiv p \land \sim q$
Proof:
	$\text{Let p and q be statements.}$
		$\text{Then,}$
			$(p \land q) \oplus p \equiv [\sim (p \land q) \land p] \lor [(p \land q) \land \sim p] \rightarrow \text{ by XOR equivalence}$
			$\equiv [(\sim p \lor \sim q) \land p] \lor [(p \land q) \land \sim p]$
			$\equiv [(\sim p \lor \sim q) \land p] \lor [p \land q \land \sim p]$
			$\equiv [(\sim p \lor \sim q) \land p] \lor [p \land \sim p \land q]$
			$\equiv [(\sim p \lor \sim q) \land p] \lor [F \land q]$
			$\equiv[(\sim p \lor \sim q) \land p] \lor F$
			$\equiv [(\sim p \lor \sim q) \land p]$
			$\equiv [(\sim p \land p) \lor (\sim q \land p)] \rightarrow \text{ by negation law}$
			$\equiv [F \lor (\sim q \land p)]$
			$\equiv \sim q \land p$
			$\equiv p \land \sim q \rightarrow \text{ by commutative law}$
	$\text{By the transitive law,}$
		$(p\land q)\oplus p \equiv p \land \sim q$
		