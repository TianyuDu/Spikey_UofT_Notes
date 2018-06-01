# ECO220 Lecture Notes May 30 2018

## Chapter 8 Probability

### 8.1 ~ 8.5 Summary

Let $A$ and $B$ be two events then

##### Addition Rule

$P(A \cup B) = P(A) + P(B) - P(A\cap B)$

##### Multiplication Rule

$P(A\cap B) = P(B) P(A \vert B) = P(A) P(B \vert A)$

##### Mutually Exclusive Event

$A \cap B = \empty$

$P(A \cap B) = 0$

$P(A \vert B) = P(A \vert B) = 0$

##### Conditional Probability

$P(A \vert B) = \frac{P(A\cap B)}{P(B)}$

##### Independent Event

$P(A \vert B) = P(A)$

$P(B\vert A) = P(B)$

$P(A \cap B ) = P(A)P(B)$

##### Example

> Toss a fair die till a 4 appress

$S = \{4, N4, NN4, NNN4, \dots\}$ Where $N \neq 4$

Let $E$ denote the collection of events that "get 4 on an event numbered trial."

Therefore $P(E) = P(\{4, NN4, NNNN4, NNNNNN4, \dots\})$

Notice that events in $E$ are *disjoint*

$= \frac{1}{6} + \frac{5}{6}\frac{5}{6}\frac{1}{6} + \dots$

$= \sum_{n=0}^\infty \frac{1}{6} \frac{5}{6}^{2n} = \frac{6}{11}$



### Bayes Theorem

Let $A$ and $B$ be two events. Suppose we know $P(A \vert B)$. Find $P(B \vert A)$

Then $P(B \vert A) = \frac{P(B) P(A \vert B)}{P(A)}$

*proof*

Since $P(A \cap B) = P(A \vert B) P(B) = P(B \vert A) P(A)$

Therefore $P(B \vert A) = \frac{P(B) P(A \vert B)}{P(A)}$

$\blacksquare$

## Chapter 9: Probability Distribution and Expected Values

