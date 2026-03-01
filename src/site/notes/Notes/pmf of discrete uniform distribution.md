---
{"dg-publish":true,"permalink":"/notes/pmf-of-discrete-uniform-distribution/","tags":["probability","statistics"]}
---

# PMF of discrete uniform distribution
The [[Notes/probability mass function\|PMF]] of a [[Notes/discrete uniform distribution\|discrete uniform distribution]] is defined as:
$$
f(x)= \frac{1}{b-a+1}
$$
where
- a represents the _lower bound_ of the distribution.
- b represents the _upper bound_ of the distribution.
- $f(x)$ is the [[Notes/probability mass function\|PMF]], representing the [[Notes/probability\|Notes/probability]] of obtaining a specific value $x$ within the range $[a,b]$.

__calculating [[Notes/probability mass function\|PMF]] of discrete uniform distribution in python__:
```python
import scipy.stats as stats
a =1
b = 6
uniform_dist = stats.randint(a,b + 1)

for value in range(a, b + 1):
	probability = uniform_dist.pmf(value)
	print(f'p(x) = {value} = {probability * 100}%')


expected output:
#<scipy.stats._distn_infrastructure.rv_discrete_frozen object at ...> p(x) = 1 = 16.666666666666664% p(x) = 2 = 16.666666666666664% p(x) = 3 = 16.666666666666664% p(x) = 4 = 16.666666666666664% p(x) = 5 = 16.666666666666664% p(x) = 6 = 16.666666666666664%

```

- the `stat.randint()` method constructs a [[Notes/discrete uniform distribution\|discrete uniform distribution]] object, which generates [[Notes/random variate\|random variates]], with a specified range.
- the returned object object from the `stat.randint()` facilitates various calculations including [[Notes/probability mass function\|PMF]].
- Then we instruct python to iterate over each value in the specified range, calculate the PMF for each value using `uniform_dist.pmf(value)`, and return the results as percentages rather than decimals
