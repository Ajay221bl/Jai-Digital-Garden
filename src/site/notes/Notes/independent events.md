---
{"dg-publish":true,"permalink":"/notes/independent-events/","tags":["probability"]}
---

# Independent Events
Two events are considered independent events if the occurrence of one event doesn't affect the occurrence of the other. 
In other words:
Knowing that one event happened gives you no information about whether the other [[Notes/event\|event]] will happen. 

The events are independent ___only if___:
	the probability of both events happening together equals the product of their individual probabilities.
- why is this true??
- $\because$ according to multiplication rule, $$P(A \cap B) = P(A|B)* P(B) $$
- we know that if $A$ and $B$ are independent then and if $B$ has already occurred it would not have any impact on the probability of event $A$.
- So, $P(A|B) = P(A)$              (__$\because$ the [[Notes/probability\|Notes/probability]] of occurrence of event A after the occurrence of event B remains as it was before the event B had occurred)__
- hence we can substitute $P(A|B)$ with $P(A) in the [[Notes/multiplication rule in conditional probability\|multiplication rule]] equation
	$$ \boxed{P(A\cap B) = P(A)*P(B)}$$


if $A$ and $B$ are independent events then if $B$ already happened there will be no change in the probability of [[Notes/event\|event]] $A$ if event $B$ has already occurred.
so in this case the [[Notes/conditional probability\|conditional probability]] $P[\,A|B\,]$ (given event B has already happened what is the probability that event A will occur) will be equal to $P(A)$ because there will be no impact of the occurrence of event B on occurrence of event A.

Lets prove it mathematically: $\boxed{P(A|B) = P(A)}$ where A and B are independent events.
- a dice and a coin are thrown together.
- the sample space in this case would be:
	- $S = \{\text{ H1, H2, H3, H4, H5, H6, T1, T2, T3, T4, T5, T6 }\}$ 
- let B is the already occurred event which is _got 3 on a dice_:
	- $\text{B = \{ H3, T3 \}}$ so $P(B) = \huge\frac{2}{12} = \frac{1}{6}$
- event A is _get heads on a coin_.
- $\text{A = \{H1, H2, H3, H4, H5, H6\}}$ 
- the [[Notes/probability\|Notes/probability]] of occurrence of event A when event B has not occurred is:
	- $P(A) = \huge\frac{6}{12} = \frac{1}{2}$
- But what is the [[Notes/probability\|Notes/probability]] of event A happening if event B has already occurred? In this case, since the events are independent, the $P[A|B] = P[A]$ and here is the proof:
	- according to [[Notes/conditional probability\|conditional probability]] formula, $$P(A|B) = \frac{P(A\cap B)}{P(B)}$$
	- $P(A\cap B) = \huge\frac{1}{12}$       and $P(B) = \huge\frac{1}{6}$
	- so $\huge{P(A|B) = \frac{P(A\cap B)}{P(B)} = \huge\frac{\huge\frac{1}{12}}{\huge\frac{1}{6}} = \huge\frac{1}{2} = P(A)}$
- __Hence, when two events A and B are independent of each other and given that B has already occurred the probability of occurring of A would remain the same as it was before the occurrence of event B.__
