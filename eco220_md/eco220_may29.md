# ECO 220 chapter 8 Probability

Let $S$ be the event space.

- $0 \leq P(A) \leq 1$
- $P(S) = 1$
- $P(A^c)  = 1 - P(A)$
- **Addition rule** $P(A\cup B) = P(A) + P(B) - P(A \cap B)$



#### Mutually Exclusive Events

**Defintion** Two events $A$ and $B$ are *multually exclusive / disjoint* iff $A \cap B = \emptyset$

**Theorem** If events $A$ and $B$ is mutually exclusive, then

​	1) $A \cap B = \emptyset \land P(A \cap B) = 0$

​	2) $P(A \cup B) = P(A) + P(B)$



## 8.2 Conditional Probability

##### Example:

> A company ships order in different days, with different qualities.

| Quality     | D1             | D2                 | D3 (And after) | Total              |
| ----------- | -------------- | ------------------ | :------------: | ------------------ |
| <u>G</u>ood | .40            | .30 $P(G\cap D_2)$ |      .10       | $P(G) = .80$       |
| <u>B</u>ad  | .10            | .05                |      .05       | $P(B) = .20$       |
| Total       | $P(D_1) = .50$ | $P(D_2) = .35$     | $P(D_3) = .15$ | $P(S) = \sum=1.00$ |

**Sample Space** $S = \{(G,D_1), (G, D_2), (G, D_3), (B, D_1), (B, D_2), (B, D_3)\}$

Where **joint probability** $P(G \cap D_2) = .30$

And **marginal probability** $P(G) = P(G \cap D_1) +  P(G \cap D_2) +  P(G \cap D_3)$ 

> Suppose a good shipment is went out. What is the probability that it is sent out in $D_2$

$P(D_2 \vert G) = \frac{P(D_2 \cap G)}{P(G)} = \frac{.3}{.8} = .375$

*The probability of $D_2​$ conditioning $G​$. Given $G​$ happens, what's the probability of $D_2​$?*