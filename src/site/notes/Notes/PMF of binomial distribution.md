---
{"dg-publish":true,"permalink":"/notes/pmf-of-binomial-distribution/","tags":["statistics","prbability"]}
---

# PMF of binomial distribution
In the context of [[Notes/binomial distribution\|binomial distributions]], the [[Notes/probability mass function\|probability mass function]]  calculates the [[Notes/probability\|Notes/probability]] of observing a specific number of successes (or failures) in a fixed number of independent trials, each with two possible outcomes.

In simple terms, it answers the questions like: "If I flip a coin 10 times, what's the probability I get exactly 7 heads"
equation:
$$
p(x=k) = \binom{n}{k}\times p^k\times(1-p)^{(n-k)}
$$
- $p(x=k)$ represents the [[Notes/probability\|Notes/probability]] of observing $k$ successes in $n$ number of trials.
- $n$ over $k$ is the [[Notes/binomial coefficient\|binomial coefficient]], also known as "n choose k", which represents the number of ways to choose $k$ successes from $n$ trials
- $p$ is the probability of success on any individual trial
- $1-p$ represents the [[Notes/probability\|Notes/probability]] of failure on any individual trial
- n is the total number of trials
- k is the number of successes

The [[Notes/probability mass function\|PMF]] for a [[Notes/binomial distribution\|binomial distribution]] is a property that characterizes the distribution and allows us to determine the probabilities associated with different number of successes.
By evaluating the [[Notes/probability mass function\|PMF]] at different values of $k$, we can obtain the [[Notes/probability distributions\|probability distribution]] for the [[Notes/binomial random variable\|binomial random variable]], thereby providing insights into the likelihood of various outcomes in a [[Notes/binomial experiment\|binomial experiment]].


#### finding [[Notes/probability mass function\|PMF]] using python
```python
import numpy as np
from scipy.stats import binom


# n is the total number of trials
n = 20

# k is the nunber of successes
k = np.arange(0, n + 1)


# p is the probability of success on any individual trial
p = [0.20, 0.50]

  

# lets pass these values to a snippet of python code that mirrors
# the probability mass equation for the binomial distribution

# we will find out the pmf values for each 
all_pmfs = []

for i in range(len(p)):
pmf = [np.math.comb(n, j) * (p[i] ** j) * ((1 - p[i]) ** (n - j)) for j in k]

all_pmfs.append(pmf)

# calculating the pmf for binomial distribution using the binom.pmf() function\
# imported from scipy.stats

n = 20
k = np.arrange(0, n+ 1)
p = [0.75, 0.90]

  

pmf = binom.pmf(k, n, p[i])
```
