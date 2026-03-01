---
{"dg-publish":true,"permalink":"/notes/finding-probability-of-a-union-b/","tags":["probability"]}
---


# Finding probability of A union B

$$A \cup B = P(A) + P(B) - P(A) \cap P(B)$$

let sample space = $\{1,2,3,4,5,6\}$

the events are:
- $A = \{1,2,3\}$
- $B = \{2,5,6\}$

$P(A) = \dfrac{3}{6} = \dfrac{1}{2}$ 

$P(B) = \dfrac{3}{6} = \dfrac{1}{2}$


$intuitively,\ P(A \cup B) = \dfrac{3}{6} + \dfrac{2}{6} = \dfrac{5}{6}$
we took $\dfrac{2}{6}$ because 2 is already there in the $event \ A$  and so we will skip it when calculating the $P(B)$

but there is a formula for calculating $P(A \cup B)$:
$$P(A \cup B) = P(A) + P(B) - P(A\cap B)$$
this formula does the same work as above automatically, by first adding the [[Notes/probability\|Notes/probability]] of both A and B and then subtracting the probability of the common part i.e. of 2 which is $\dfrac{1}{6}$

$$P(A\cup B) = \dfrac{3}{6} + \dfrac{3}{6} - \dfrac{1}{6} = \dfrac{5}{6}$$
