---
{"dg-publish":true,"permalink":"/notes/cumulative-distribution-function/","tags":["statistics","probability"]}
---

# cumulative distribution function

it is a function that gives the [[Notes/probability\|Notes/probability]] that a random variable takes on a value up to and including the given value x. The [[Notes/cumulative distribution function\|CDF]] is derived by adding up the probabilities given by the [[Notes/probability density function\|PDF]]. 
![Pasted image 20250731223011.png](/img/user/Notes/Pasted%20image%2020250731223011.png)

the CDF, typically denoted as $F(x)$ or $P(X\leq{x})$, gives the probability that a continuous random variable $X$ takes on a value less than or equal to a given point $x$.

- The function $F(x)$ is non-decreasing (also called monotonically increasing). that is, as x increases, the probability P(X<= x) does not decrease. It will either increase or stabilize; but as a CDF, it does not and cannot ever decrease. so if $a<{b}$ then $F(a) \leq{F(b)}$
- The value of $F(x)$, as a probability, is always equal to some value between 0 and 1; therefore $0\leq{\text{   F(x)  }\leq{1}}$ 


> In the above graph, when the [[Notes/random variable\|random variable]] equals 4.5, the [[Notes/cumulative distribution function\|CDF]] equals 70%. This means that the probability of a random variable value being less than or equal to 4.5 is about 70%.


> The [[Notes/cumulative distribution function\|CDF]] 
```dataview
list
from 
where file.ctime >= date(today) - dur(10 day)
sort file.ctime asc

```
