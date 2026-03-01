---
{"dg-publish":true,"permalink":"/notes/z-score-table/","tags":["statistics","probability"]}
---

# z-score table
it is a table that holds the [[Notes/probability\|Notes/probability]] values associated with [[Notes/z-score\|z-scores]].

The table provides the the area under the standard normal curve to the left of a given [[Notes/z-score\|z-score]], which corresponds to the cumulative probability (see [[Notes/cumulative distribution function\|CDF]])


![Pasted image 20250802155833.png](/img/user/Notes/Pasted%20image%2020250802155833.png)

-  the far-left column indicates the first two digits of the z-table
- the top row indicates the next two digits of the z-score

a [[Notes/z-score\|z-score]] of 1 for instance is equivalent to 1.0000. The corresponding probability (or the value of [[Notes/cumulative distribution function\|CDF]] to be precise) could be found out by finding the intersection of the 1.0 in the left-most column and the 0.0 value in the top row.
Hence the corresponding cumulative probability is therefore equal to $.8413$ or $84.13\%$ 


the respective probability could also be calculated in [[Notes/python\|python]] using the norm instance which is located inside the stat module of scipy library
```python
from scipy.stats import norm
z=1

# cdf stands for cumulative distribution function
first_probability = norm.cdf(z)

print(f"Probability (area): {first_probability * 100}%")
z = 1.5

second_probability = norm.cdf(z)
print(f"Probability (area): {second_probability * 100}%")
 

range_probability = second_probability - first_probabilit
print(f"Probability (area): {range_probability * 100}%")
```
