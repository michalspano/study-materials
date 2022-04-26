Prove that $\sqrt 7$ is irrational.

$$S: \sqrt 7 \in \mathbb{Q'}$$
$$\neg S: \sqrt 7 \in \mathbb{Q}$$

We prove $S$ by **contradiction**. That is:

Suppose $S$;
$\neg S \rightarrow N \mid S$, where $N$ is some **nonsense**.

We assume $\sqrt 7$ to be rational,  that implies $\sqrt 7 = \dfrac{p}{q}$, where $p \in \mathbb{Z} \land q \in \mathbb{Z}-\{0\}$ and that $p,q$ are relatively prime, i.e. coprime integers $\Rightarrow \nexists d \in \mathbb{N}-\{1\}: d \mid p \land d \mid q$.

$\sqrt 7 = \dfrac{p}{q}$
$7 = \Big( \dfrac{p}{q} \Big)^{2}$
$7 = \dfrac{p^2}{q^2}$
$7 q^{2}= p^{2} \Rightarrow 7 \mid p^{2}$

**Assumption:** $7 \mid p^{2} \Rightarrow 7 \mid p$

$$A: 7 \mid p^{2} \Rightarrow 7 \mid p$$
$$A': 7 \nmid p \Rightarrow 7 \nmid p^{2}$$

Let $p = 7a + 1$, where $a \in \mathbb{Z}$: $p^{2}= (7a + 1)^{2} \dots 7\times(7 a^{2}+ 7a) + 1$. Let $(7 a^{2}+ 7a) = z \Rightarrow 7z + 1 \Rightarrow 7 \nmid 7z + 1 \Rightarrow 7 \nmid p^2$. The assumptions is **true**.

Thus, $7 \mid p^{2} \Rightarrow 7 \mid p \Rightarrow p=7a$, where $a \in \mathbb{Z}$.

$7q^{2}=(7a)^{2}$
$7q^{2}=49a^{2}$
$q^{2}=7a^{2} \Rightarrow 7 \mid q^{2} \Rightarrow 7 \mid q$

**Contradiction with the assumption**: $p,q$ are not relatively prime, symbolically: $\exists d \in \mathbb{N}-\{1\}: d \mid p \land d \mid q \Rightarrow \sqrt 7 \neq \dfrac{p}{q} \Rightarrow \sqrt 7 \notin \mathbb{Q} \Rightarrow \sqrt 7 \in \mathbb{Q'}$.

**Conclusion**: $\sqrt 7$ is an **irrational** number.
