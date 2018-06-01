# ECO 220 chapter 8 Probability

Let $S$ be the event space.

- $0 \leq P(A) \leq 1$
- $P(S) = 1$
- $P(A^c)  = 1 - P(A)$
- **Addition rule:** $P(A\cup B) = P(A) + P(B) - P(A \cap B)$



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

*The probability of $D_2$ conditioning $G$. Given $G$ happens, what's the probability of $D_2$?*

In general, if $A$ and $B$ are events in sample space $S$, define **conditional probability** of $A$ given $B$ as $P(A \vert B) = \frac{P(A \cap B)}{P(B)}$

Similarly, $P(B \vert A) = \frac{P(A \cap B)}{P(A)}$

**Multiplication Rule:**

$P(A \cap B) = P(A \vert B) \times P(B) = P(B \vert A) \times P(A)$

##### Example

> $P(A) = .3$ , $P(B) = .4$

a) $P(A \cup B) = P(A) + P(B) - P(A \cap B) = .7 - P(A \cap B)$

b) *If A and B are disjoint* $P(A \cup B) = P(A) + P(B) - P(A \cap B) = .3 + .4 - .0 = .7$

c) If $P(B \vert A) = .2$, $P(A \cup B) = P(A) + P(B) - P(A \cap B) = .7 - (P(B\vert A) \times P(A)) = .7 - .2 * .3 = .64$

d) If $A, B$ are disjoint, then $P(B \vert A) = 0$



## Independent Event

##### Example

> Let $A$ be the event that student $A$ passes, $B$ be the event that student $B$ passes.

a) Events $A$ and $B$ **independent** means $A$ has <u>no</u> impact on prob of $B$. That's

$P(A \vert B) = P(A)$, or $P(B \vert A) = P(B)$

Or $P(A \cap B) = P(A \vert B) P(B) = P(A) P(B)$

b) If $A$ and $B$ are mutually exclusive

When $A$ occurs, $B$ will not occur, and vice versa.

Therefore $P(A\vert B) = P(B \vert A) = P(A \cap B) = 0$

Therefore **If two events are independent, they could not be mutually exclusive.**

**If two events are mutually, they could not be independent**

##### Definition of independence (three equivalent definitions)

1) $P(A \vert B) = P(A)$ or

2) $P(B \vert A) = P(B)$ or 

3) $P(A \cap B) = P(A)P(B)$

