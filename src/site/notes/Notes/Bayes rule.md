---
{"dg-publish":true,"permalink":"/notes/bayes-rule/","tags":["probability"]}
---

# Bayes rule
Bayes rule help us flip the [[Notes/conditional probability\|conditional probability]] to calculate the unknown [[Notes/probability\|Notes/probability]].

Bayes rule formula:
$$P(A|B) = \frac{P(A\cap B)}{P(B)}$$
how can we find $P(B|A)$ ?
$$P(B|A) = \frac{P(B \cap A)}{P(A)}$$

since $P(A\cap B) == P(B \cap A)$, we can do the following according to [[Notes/multiplication rule in conditional probability\|multiplication rule in conditional probability]]

$$P(B\cap A) = P(A|B) \times P(B)$$
$$\boxed{P(B\ |\ A) = \frac{P(A \ | \ B ) \times P(B)}{P(A)}}$$
Implementing it on an example:
$P(listening \ Rap)*P(listening \ to \ tupac \ | \ listening \ Rap) = P(listening \ to \ tupac)\; * \; P(listening \ Rap \ | \ listening \ to \ tupac)$
$$P(listening \ to \ tupac \ | \ listening \ Rap) = \frac {P(listening \ to \ tupac)*P(listening \ Rap \ | \ listening \ tupac)} {P(listening \ Rap)}$$
in the above equation, we can  find the probability of user listening to tupac, given he listened the Rap genre.
