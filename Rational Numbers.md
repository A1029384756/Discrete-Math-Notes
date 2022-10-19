<b>Def:</b> $\mathbb{Q} = \{ \frac{a}{b} | a, b \in \mathbb{Z} \land b \neq 0\}$
<b>Def:</b> $\forall x \in \mathbb{R}, x \text{ rational} \leftrightarrow x \in \mathbb{Q}$
<b>Def:</b> $\forall x \in \mathbb{R}, x \text{ rational} \leftrightarrow x \in \mathbb{Q}$
<b>Def:</b> $\frac{a}{b}+\frac{c}{d} = \frac{ad + cb}{bd}$
<b>Def:</b> $\frac{a}{b} = \frac{c}{d} \leftrightarrow ad = cb$

><b>Important Note:</b> The representation of a rational number as $\frac{a}{b}$ is not unique.

<b>Ex.</b> $\frac{3}{4} = \frac{9}{12} = \frac{-27}{-36} = \frac{1}{1.\overline{333}}$
<b>Ex.</b> $\frac{\pi}{3\pi} = \frac{1}{3}$
Writing a number as $\frac{a}{b}$ where the top and bottom aren't integers, is NOT a proof that the number is irrational.

><b>Also:</b> If $\frac{a}{b} = \frac{c}{d}$ that does not mean that $a = c$ or $b = d$ necessarily.

<b>Point:</b> Showing that $a \neq c$ or $b \neq d$ is NOT proof that $\frac{a}{b} \neq \frac{c}{d}$, ex: $\frac{1}{2} = \frac{5}{10}$

<b>Claim:</b> $\forall a \in \mathbb{Z}, \exists b \in \mathbb{Z} | \frac{a}{b} = \frac{1}{2}$
	Negation: $\exists a \in \mathbb{Z}| \forall b \in \mathbb{Z}, \frac{a}{b} \neq \frac{1}{2}$
	<u>Scratch Work:</u> $\frac{0}{b} = 0 \neq \frac{1}{2} \forall b$
	<u>Disproof:</u> Let $a = 0$.
	Note, $a = 0 \in \mathbb{Z}$ as required.
	Further, WTS $\forall b \in \mathbb{Z}, \frac{0}{b} \neq \frac{1}{2}$
	Let $b$ be any arbitrary but particular integer.
	Note, $b = 0$ or $b \neq 0$. Proceed by division into cases.
	<u>Case 1:</u> $b = 0$ Then, $\frac{0}{0}$ D.N.E., thus cannot be $\frac{1}{2}$.
	<u>Case 2:</u> $b \neq 0$. Then consider $\frac{0}{b}$ and $\frac{1}{2}$.
	Note, $0 * 2 = 0$.
	Note $\frac{0}{b} = 0 \neq \frac{1}{2}$.
	Thus, by direct proof, $\forall b \in \mathbb{Z}, \frac{0}{b} \neq \frac{1}{2}$.
	Therefore, by example,
		$\exists a \in \mathbb{Z} | \forall b \in \mathbb{Z}, \frac{a}{b} \neq \frac{1}{2}$

<u>Def:</u> $\mathbb{Z*} = \{\text{non-zero integers}\} = \{n \in \mathbb{Z} | n \neq 0\}$
<u>Def:</u> $\mathbb{Q*} = \{\text{non-zero rationals}\} = \{\frac{a}{b} | a,b \in \mathbb{Z} \land a,b \neq 0\}$
<u>Def:</u> $\mathbb{R*} = \{\text{non-zero real numbers}\}$
<b>Claim:</b> $\forall a \in \mathbb{Z*}, \exists b \in \mathbb{Z} | \frac{a}{b} = \frac{1}{2}$.
	Negation: $\exists a \in \mathbb{Z*}| \forall b \in \mathbb{Z}, \frac{a}{b} \neq \frac{1}{2}$
	<u>Proof:</u> Let $a$ be any arbitrary but particular integer.
	- WTS $\exists b | \frac{a}{b} = \frac{1}{2}$
	- Let $b = 2 * a$.
	- Note, as $2, a \in \mathbb{Z}$ we know $2a \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $*$.
	- Further, WTS $\frac{a}{b} = \frac{1}{2}$.
	- Note since $a * 2 = 2a$ by commutative property of $*$.
	- $a*2 = b$ by substitution
	- $a*2 = b*1$ by evaluation.
	- Hence, as $a*2 = b*1$, $\frac{a}{b} = \frac{1}{2}$ by definition of rational equality.
	Thus, by example $\exists b | \frac{a}{b} = \frac{1}{2}$.
	Therefore, by direct proof, $\forall a \in \mathbb{Z*}, \exists b \in \mathbb{Z} | \frac{a}{b} = \frac{1}{2}$.

<b>Claim:</b> $\mathbb{Q}$ is closed under $\div$.
<u>Logic:</u> $\forall x, y \in \mathbb{Q}, \frac{x}{y} \in \mathbb{Q}$
<u>Negation:</u> $\exists x, y, \in \mathbb{Q} | \frac{x}{y} \notin \mathbb{Q}$
<u>Disproof:</u> Let $x = 1$ and $y = 0$.
	- Note, as $x = 1 = \frac{1}{1}$ and $y = 0 = \frac{0}{1}$, $x$ and $y$ in $\mathbb{Q}$ as desired.
	- Further, $\frac{x}{y} = \frac{1}{0}$ which does not exist.
	- Hence, $\frac{x}{y} \notin \mathbb{Q}$ as desired.
	- Thus, by example, $\exists x, y, \in \mathbb{Q} | \frac{x}{y} \notin \mathbb{Q}$.

<b>Claim:</b> $\mathbb{Q*}$ is closed under $\div$.
<u>Logic:</u> $\forall x, y \in \mathbb{Q*}, \frac{x}{y} \in \mathbb{Q*}$
<u>Negation:</u> $\exists x, y, \in \mathbb{Q*} | \frac{x}{y} \notin \mathbb{Q*}$
<u>Proof:</u> Let $x$ and $y$ be any arbitrary but particular non-zero rational number.
	- Since $x \in \mathbb{Q*}$ we know $x = \frac{a}{b}$ for some $a, b \in \mathbb{Z}$ with $a, b \neq 0$ by definition of $\mathbb{Q*}$.
	- Further, as $y \in \mathbb{Q*}$ we know $y = \frac{c}{d}$ for some $c, d \in \mathbb{Z}$ with $c, d \neq 0$ by definition of $\mathbb{Q*}$.
	- Consider $\frac{x}{y}$. 
	- Note, $\frac{x}{y} = \frac{\frac{a}{b}}{\frac{c}{d}}$ by subsitution.
	- $\frac{x}{y} = \frac{a}{b} * \frac{d}{d}$ by flip and multiply rule.
	- $\frac{x}{y} = \frac{ad}{bc}$ by rational multiplication.
	- Note, since $a, b, c, d \in \mathbb{Z}$, $ad, bc \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $*$.
	- Further, as $a,b,c,d \neq 0$ $ad \neq 0$ and $bc \neq 0$, by the Zero product propery.
	- Thus, since $\frac{x}{y} = \frac{ad}{bc}$ where $ad, bc \in \mathbb{Z}$ and $ad,bc \neq 0$, $\frac{x}{y} \in \mathbb{Q*}$, by def of $\mathbb{Q*}$.
	- Therefore, by direct proof, $\forall x,y \ in \mathbb{Q*}, \frac{x}{y} \in \mathbb{Q*}$.

> <b>Fact:</b> Zero Product Property
> $ab = 0 \leftrightarrow a = 0 \lor b = 0 \equiv ab \neq 0 \leftrightarrow a \neq 0 \land b \neq 0$