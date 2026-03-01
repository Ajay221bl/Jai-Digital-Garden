---
{"dg-publish":true,"permalink":"/notes/mutually-exclusive-events-are-not-independent/","tags":["probability"]}
---

# [[Notes/mutually exclusive sets or events\|mutually exclusive events]] are not [[Notes/independent events\|independent]]


Proof:
if event A and event B are [[Notes/mutually exclusive sets or events\|mutually exclusive]] it means $P(A \cap B) = \{\,\,\}$ or $P(A\cap B) = 0$

lets find if $A$ and $B$ are independent. $A$ and $B$ will be independent if 
$P(A|B) = P(A)$
lets find $P(A|B) in this case.
According to [[Notes/conditional probability\|conditional probability]] formula, $P(A|B) = \huge\frac{P(A\cap B)}{P(B)}$
- in this case $\huge P(A|B) = 0$      (since $P(A\cap B) = 0$)
- so $P(A|B) \neq P(A)$

### intuitive explanation
- suppose a die is rolled
- $\text{S= \{1 ,2, 3, 4, 5, 6\}}$
- events:
	- $\text{event A = getting a 2}$
	- $\text{event B = getting a 6}$
	- ___both of the above events are mutually exclusive___
- $A$ and $B$ are not independent because they __influence the [[Notes/probability\|Notes/probability]] of each other.__
	- suppose if die is thrown and we get a 6, then the $P(\text{getting a 2)}$ becomes zero for the same roll
	- and if we get a 2 on the die roll, then the $P(\text{getting a 6})$ becomes zero for the same roll.
	- so both events are influencing the [[Notes/probability\|Notes/probability]] of each other.
