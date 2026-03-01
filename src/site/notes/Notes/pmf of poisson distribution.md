---
{"dg-publish":true,"permalink":"/notes/pmf-of-poisson-distribution/","tags":["statistics","probability"]}
---

# [[Notes/probability mass function\|PMF]] of [[Notes/poisson distribution\|poisson distribution]]
the [[Notes/probability mass function\|PMF]] for the [[Notes/poisson distribution\|poisson distribution]] models the [[Notes/probability\|Notes/probability]] of observing a specific number of events within a fixed interval of time or space, given the average rate at which those events occur.
It uses the frequency of recorded events to estimate the rate at which the same events should occur in a future interval of time or space.eee

$$
P(X=k) = \frac{e^{ -\lambda}\lambda^{x}}{x!}
$$
where:
- $P(X=x)$ is the [[Notes/probability\|Notes/probability]] of observing $k$ [[Notes/event\|events]]
- $e$ is the base of the [[natural logarithm\|natural logarithm]], approximately equal to $2.72$.
- $\lambda$ (lambda) is the average rate of occurrence (also known as the [[Notes/rate parameter\|rate parameter]]mber of events

Its often obsereved that the [[Notes/probability mass function\|PMF]] for the [[Notes/poisson distribution\|poisson distribution]] includes the [[Notes/mean\|mean]] ($\mu$) rather than the rate parameter ($\lambda$). However this discrepancy is inconsequential because in the [[Notes/poisson distribution\|poisson distribution]], both the mean and the [[Notes/variance\|variance]] ($\sigma^{2}$) are equal to the [[Notes/rate parameter\|rate parameter]].
Hence:
$$
\mu = \sigma^{2}= \lambda
$$
##### calculating the [[Notes/probability mass function\|PMF]] for [[Notes/poisson distribution\|poisson distribution]] in python
```python
from scipy.stats import poisson
lam = 2
k = 4
probability_formula= poisson.pmf(l, lam)

print(f"Probability (using python method): {probability_formula * 100}%' )
```
