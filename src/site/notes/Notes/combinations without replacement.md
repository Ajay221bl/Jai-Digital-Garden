---
{"dg-publish":true,"permalink":"/notes/combinations-without-replacement/","tags":["combinatorics","probability"]}
---

# combinations without replacement

first think about the [[Notes/permutation without replacement\|permutation without replacement]] and then insert an adjustment to eliminate the significance of order because the order doesn't matter in case of combinations.

the number of [[Notes/combination\|combinations]] is always less that the number of [[Notes/permutation\|permutations]] because in combinations the order doesn't matter and 1-2-3, 2-3-1, 3-2-1 are one and same.


lets take an example where $n=5$ and $r=3$

the permutations without replacement in this case would be:
${5}\times{4}\times{3}= 60$
since the _order matters_ in [[Notes/permutation\|permutations]], the number of ways the three digits can be sequenced is $3! \text{ which is 6}$.

this means permutations without replacement have six times as many possible outcomes as combinations without replacement when $n=5$ and $r=3$.

hence, we adjust the [[Notes/permutation without replacement\|permutation without replacement]] formula to reduce it by an order of magnitude equal to the number that was just calculated, because we no longer care about the order

permutations without replacement formula: $$\frac{n!}{(n-r)!}$$


combinations without replacement formula derived from [[Notes/permutation without replacement\|permutation without replacement]] formula:
$$
\frac{\text{permuation without replacement formula}}{r!}
$$
$$
=\frac{n!}{r!(n-r)!} = \frac{5!}{3!(5-3)!} = \frac{120}{12} = 10
$$
