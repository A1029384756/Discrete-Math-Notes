<b>Def:</b> $\forall a, b \in \mathbb{Z}, a| b \leftrightarrow [\exists k \in \mathbb{Z} | ak = b]$
>$a | b \equiv \text{ "a divider b" : "b is divisible by a" : "b is a multiple of a"}$

<u>Ex:</u> 
- $7 | 21$ since $7*3 = 21$
- $6 | -12$ since $6(-2) = 12$
- $5 | 0$ since $5*0 = 0$
Anything divides $0 \equiv 0$ is a multiple of anything.
- $0 \nmid 7$ since $0*\text{anything} = 0 \neq 7$

> What happens with 0?
> - Either undefined because no $k$ exists or because infinitely many $k$ exist.

<b>Claim:</b> $\forall a,b,c \in \mathbb{Z}, c| a \land c | b \rightarrow c|a + b$
<b>Negation:</b> $\exists a,b,c \in \mathbb{Z} | c | d \land c | b| \land c \nmid a + b$

<b>Proof:</b> Let $a$, $b$, and $c$ be any arbitrary but particular integers.
Suppose $c | a \land c | b$.
Since $c|a$, there is some $k \in \mathbb{Z}, a = ck$, by definition of divisibility.
Since $c|b$, there is some $l\in \mathbb{Z}, b = cl$, by definition of divisibility.
Consider, $a+b$, WTS $a+b=c$ times some integer.
Note, $a+b=c*k+c*l$, by substitution.
	$a+b = c(k + l)$, by factoring.
Note, since $k, l \in \mathbb{Z}$, we know $k+l \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $+$.
Thus, as $a+b=c(k+l)$ where $k+l \in \mathbb{Z}$, we can deduce $c|a + b$ by definition of divisibility.
Therefore, by direct proof $\forall a,b,c \in \mathbb{Z}, c|a \land c|b \rightarrow c|a + b$.

<b>Claim:</b> $\forall a,b,c \in \mathbb{Z}, c|a \rightarrow c|(a*b)$

<b>Proof:</b> Let $a,b,c$ be arbitrary but particular elements of $\mathbb{Z}$.
Assume $c|a$.
Sincd $c|a$, we know $a=c*k$ for some $k \in \mathbb{Z}$, by definition of divisibility.
Consider $a*b$. WTS $a*b=c$ times some integer.
Note, $a*b =(c*k)*b$ by substitution.
	$a*b=c*(k*b)$ by associative law.
Note, since $k,b \in \mathbb{Z}$, $k*b \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $*$.
Thus, $a*b=c*(k*b)$ with $k*b \in \mathbb{Z}$, $c|(a*b)$ by definition of divisibility.
Therefore, by direct proof,
	$\forall a,b,c \in \mathbb{Z}, c|a \rightarrow c|(a*b)$.

