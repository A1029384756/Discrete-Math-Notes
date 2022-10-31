[[Mathematical Proofs]]

<b>Claim:</b> $\forall n \in \mathbb{Z}, n^2 \text{ even } \rightarrow n \text { even}$
<b>Scratch Work:</b>
- $n^2 \text{ even } \Rightarrow n^2 = 2k$ for some integer $k$.
- Consider $n$.
- Cannot go much further using [[Direct Proof]] 

><b>Idea:</b> Remember a conditional statement is always equivalent to its [[Conditional Statements#^9b0b4f|contrapositive]]

<b>Proof:</b>
- Proof by contrapositive (contraposition). Note the contrapositive is $\forall n \in \mathbb{Z}, n \text{ odd } \rightarrow n^2 \text{ odd}$.
- Let $n$ be any arbitrary/particular integer.
- Assume $n$ is odd.
- Since $n$ is odd, $n = 2k + 1$ for some $k \in \mathbb{Z}$, by definition of odd.
- Consider $n^2$. WTS $n^2$ is odd.
- $n^2 = (2k+1)^2$ by substitution.
- $n^2 = 4k^2+2k+2k+1$ by distribution.
- $n^2 = 4k^2 + 4k + 1$ by simplification.
- $n^2=2(2k^2+2k)+1$ by simplification.
- Note, as $2,k \in \mathbb{Z}$, $2k^2+2k \in \mathbb{Z}$ by closure of $\mathbb{Z}$ under $+$ and $*$.
- Thus, as $n^2 = 2(2k^2+2k)+1$ with $2k^2+2k \in \mathbb{Z}$, $n^2$ odd by definition.
- Therefore, by direct proof, $\forall n \in \mathbb{Z}, n \text{ odd } \rightarrow n^2 \text{ odd}$.
- Hence, by contrapositive, $\forall n \in \mathbb{Z}, n^2 \text{ even } \rightarrow n \text { even}$.

- [[Proof by Contrapositive]]
- [[Proof by Contradiction]]
