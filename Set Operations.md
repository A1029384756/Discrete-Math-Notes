Operations for [[Sets]]
Ways to form a new set from existing sets.

**Union:** $A \cup B = \{x | x \in A \lor x \in B\}$
$\{1,2,3\} \cup \{1,3,7\} = \{1,2,3,7\}$

**Intersection:** $A \cap B \{x | x\in A \land x \in B\}$
$\{1,2,3\} \cup \{1,3,7\} = \{1\}$

**Symmetric Difference:**  $A \dot{-} B = \{x|x\in A \oplus x \in B\}$
$\{1,2,3\} \cup \{1,3,7\} = \{2, 7\}$

**Set Difference:** $A-B = \{x|x\in A \land x \notin B\}$
$\{1,2,3\} \cup \{1,3,7\} = \{2\}$

**Set Complement:** $A^c = \{x|x \in U \notin A\}$

## Set Expressions
More complex sets built from simpler sets using set operations.
**Ex.** $(\mathbb{Z} \cap A)^c - \mathbb{Q}$

>**Set Identities:** Two set expressions are equal if the resulting sets are equal for anything you plug into the variables.
>**Ex.** $(A \cap B)^C = A^C \cup B^C$

### How to Prove Two Sets are Equal
**Finite Sets:** Brute force check to make sure both sets contains the same elements.
**Infinite Sets:** Go back to definition of what it means for two sets to be equal...
> $A = B \leftrightarrow A \subseteq B \land B \subseteq A$

#### Double Set Containment
**Idea:** Show $A=B$ by using the element method twice. Once to show $A \subseteq B$ and again to show $B \subseteq A$. Then, we can conclude $A=B$. This form of reasoning is known as Proof by Double Set Containment.

**Ex.** *Claim:* $(\mathbb{R} - \mathbb{Q}) \cup \{0\} = T = \{ab | a \in \mathbb{Q} \land b \in \mathbb{R} - \mathbb{Q}\}$
Proof by Double Set Containment, WTS $\rightarrow$ $(\mathbb{R} - \mathbb{Q}) \cup \{0\} \subseteq T \land (\mathbb{R}-\mathbb{Q}) \cup \{0\} \supseteq T$
($\subseteq$), WTS $\forall x \in \mathbb{R}-\mathbb{Q} \cup \{0\}, x \in T$
	- Let $x$ be any arb/part element in $(\mathbb{R}-\mathbb{Q}) \cup \{0\}$.
	- $x \in (\mathbb{R}-\mathbb{Q}) \cup \{0\} \Rightarrow x \in \mathbb{R} - \mathbb{Q} \land x \in \{0\}$ by definition of $\cup$.
	- *Case 1:* $x \in \{0\}$. Since $x \in \{0\}$, $x$ must equal $0$.
		- WTS $x \in T$, i.e. $x = ab$ where $a \in \mathbb{Q}$ and $b \in \mathbb{R} - \mathbb{Q}$
		- Note, $x=0=0* \pi$ with $0 \in \mathbb{Q}$ and $\pi \in \mathbb{R} - \mathbb{Q}$
		- Thus, $x \in T$ by definition of $T$.
	- *Case 2:* $x \in \mathbb{R} - \mathbb{Q}$. WTS $x \in T$, i.e., $x=ab$ with $a \in \mathbb{Q} \land b \in \mathbb{R} - \mathbb{Q}$
		- Note, $x = 1*x$ with $1 \in \mathbb{Q}$ and $x \in \mathbb{R} - \mathbb{Q}$. 
		- Thus, $x \in T$ by definition of $T$.
	Hence, by division into cases, $x \in T$.
	Thus, by the element method, $(\mathbb{R}-\mathbb{Q}) \cup \{0\} \subseteq T$
($\supseteq$) WTS $\forall a \in T, x \in (\mathbb{R}-\mathbb{Q})\cup\{0\}$
	-Let $x$ be any arb/part element of $T$.
	- Since $x \in T$, $x = ab$ for some $a \in \mathbb{Q}$ and some $b \in \mathbb{R}-\mathbb{Q}$.
	- Note, $a = 0$ or $a \neq 0$, proceed by division into cases:
	- *Case 1:* $a = 0$. Then, $x = a*b = 0*b = 0$.
		- Since $x = 0$, $x \in \{0\}$.
		- Then, $x \in \{0\} \Rightarrow x \in \{0\} \lor x \in \mathbb{R} - \mathbb{Q}$, by generalization.
		- As $x \in \{0\} \lor x \in \mathbb{R} - \mathbb{Q} \Rightarrow x \in \mathbb{R} - \mathbb{Q} \cup \{0\}$ by definition of $\cup$.
	- *Case 2:* $a \neq 0$. WTS $x \in (\mathbb{R}-\mathbb{Q}) \cup \{0\}$. Consider $x$.
		- Since $x=ab$ with $a \in \mathbb{Q^*}$ and $b \in \mathbb{R} - \mathbb{Q}$, $x \in \mathbb{R} - \mathbb{Q}$, by fact from class.
		- As $x \in \mathbb{R} - \mathbb{Q}$, $x \in (\mathbb{R}-\mathbb{Q}) \cup \{0\}$ by definition of $\cup$.
	Thus, by division into cases, no matter the $a$, $x \in (\mathbb{R}-\mathbb{Q})\cup \{0\}$.
	Hence, by element method, $(\mathbb{R} - \mathbb{Q})\cup \{0\} \supseteq T$.
Therefore, by double set containment, $(\mathbb{R} - \mathbb{Q}) \cup \{0\} = T = \{ab | a \in \mathbb{Q} \land b \in \mathbb{R} - \mathbb{Q}\}$.

> We can show that two expressions are always equal using this double set containment method.

**Claim:** $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$
**Proof:** WTS $A \cap (B \cup C) \subseteq (A \cap B) \cup (A \cap C) \land A \cap (B \cup C) \supseteq (A \cap B) \cup (A \cap C)$
($\subseteq$) WTS $\forall x \in A \cap (B \cup C), x \in (A\cap B)\cup (A \cap C)$
	- Let $x$ be any arb/part element in $A \cap (B \cup C)$.
	- Thus, $x \in A \cap (B \cup C) \Rightarrow x \in A \land x \in B \cup C$ by definition of $\cap$.
	- $\Rightarrow x \in A \land (x \in B \lor x \in C)$ by definition of $\cup$.
	- $\Rightarrow (x \in A \land x \in B) \lor (x \in A \land x \in C)$, by distributive law for logic.
	- $\Rightarrow (x \in A \cap B) \lor (x \in A \cap C)$, by definition of $\cap$.
	- $\Rightarrow x \in (A \cap B) \cup (A \cap C)$ by definition of $\cup$.
	- Thus, by the element method, $A \cap (B \cup C) \subseteq (A \cap B) \cup (A \cap C)$.
($\supseteq$) WTS $\forall x \in (A \cap B) \cup (A \cap C), x \in A \cap (B \cup C)$.
	- Same thing here!

> Can also use set laws and identities to avoid use double set containment

