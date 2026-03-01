---
{"dg-publish":true,"permalink":"/notes/complement-rule-for-probability/","tags":["statistics","probability"]}
---

# complement rule for probability
the [[Notes/probability\|Notes/probability]] of the complement of an event is equal to 1 minus the probability of the event itself.

$$
 P(A^{C}) = 1- P(A)
$$
> this rule is particularly useful when dealing with scenarios where it is easier to determine the [[Notes/probability\|Notes/probability]] of complement, or inverse, rather than the event itself, allowing for more efficient probability computations and problem-solving strategies.


for example:
we need to find the [[Notes/probability\|Notes/probability]] of getting a 4 on at least one of two dice rolls.
what does that mean? it means that:
- having a 4 on dice1 and some other number on dice2 is good
- having some number on dice1 and a 4 on the dice2  is good
- having 4 on both dice1 and dice2 is good

all three are [[Notes/mutually exclusive sets or events\|mutually exclusive]] events so we will apply the [[Notes/addition rule\|addition rule]] to find the total probability of the above three cases to find the probability of getting a 4 on at least one of two dice.

$P(\text{getting a 4 on D1 and some other number on D2})=\large{\frac{5}{36}}$
$\text{P(getting some other number on D1 and 4 on D2)} = \large{\frac{5}{36}}$
$P(\text{getting 4 on both die})=\large{\frac{1}{36}}$

$P(\text{getting 4 on atleast one of the dice})=\large{\frac{5}{36}+ \frac{5}{36}+ \frac{1}{36}=\frac{11}{36}}$

we had to find three [[Notes/probability\|probabilities]] in order to find the required probability.

>what if we could do it in an easier way? why not find the compliment of getting a 4 on at least one of dice

the complement in this case would be $P(\text{getting 4 on neither of die})$

we will use [[Notes/multiplication rule\|multiplication rule]] to find out the $P(\text{getting 4 on neither of the die})$ 

$P(\text{getting 4 on neither of the dice}) = P(\text{getting number other than 4 on dice 1})\times{P(\text{getting number other than 4 on dice 2 }})$
$P(\text{getting 4 on neither of die}) = \large{\frac{5}{36}\times{\frac{5}{36}}} = \frac{25}{36} = 69\%$
hence:
$P(\text{getting 4 on atleast one of the die}) = 1- P(\text{getting 4 on neither of the die})$

$P(\text{getting 4 on atleast one of the die})= 31\%$
