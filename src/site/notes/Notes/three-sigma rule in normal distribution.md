---
{"dg-publish":true,"permalink":"/notes/three-sigma-rule-in-normal-distribution/","tags":["statistics","probability"]}
---

# three-sigma rule in [[Notes/normal distribution\|normal distribution]]

> 68-95-99 rule

it is called three sigma because the rule talks about three [[Notes/standard deviation\|standard deviations]] 

The rule states that:
- approximately $68\%$ of the data in the [[Notes/normal distribution\|normal distribution]] is within one [[Notes/standard deviation\|standard deviation]] of the [[Notes/mean\|mean]].
- approximately $95\%$ of the data is within two [[Notes/standard deviation\|standard deviations]] of the [[[mean\|[mean]]
- upto $99.7\%$ of the data is within three [[Notes/standard deviation\|standard deviations]] of the mean.


![Pasted image 20251023135940.png|400](/img/user/Notes/Pasted%20image%2020251023135940.png)
------
### example:
suppose that the scores on an achievement test given to all high school seniors in a state are known to have, approximately, a [[Notes/normal distribution\|normal distribution]] with [[Notes/mean\|mean]] $\mu = 64$ and [[Notes/standard deviation\|standard deviation]] $\sigma=10$.
- It can then be deduced that approximately $68\%$ of the scores are between $64 - 10$ which is $54$ and $64 + 10$ which is $74$. (because $\mu \pm \sigma$)
- That approximately $95\%$ of the scores are between $44$ and $84$. (because $\mu \pm {2}\sigma$)
- and almost all the scores are between $34$ and $94$. (because $\mu \pm3\sigma$)








##### validating three sigma rule in python
```python
mean = 0
std_dev = 1
import numpy as np

# generating random samples from standard normal distribution
samples = np.random.normal(mean, std_dev, 10000)

  
  

# calculating absolute differences between each sample in the sample array and mean
np.abs(samples - mean)

  

# finding if each absolute difference value is less than the std_dev (which is 1 in this case)
# the np.sum() sums up all the Boolean values (True = 1 and False = 0)
# so the variable within_1_std holds the value of number of samples in one standard deviation

within_1_std = np.sum(np.abs(samples-mean) < std_dev)
within_2_std = np.sum(np.abs(samples- mean) < 2* std_dev)
within_3_std = np.sum(np.abs(samples -mean) < 3 * std_dev)

  

print(f"within 1 standard deviation: {within_1_std /100}%")
print(f"within 2 standard deviation: {within_2_std/100}%")
print(f"within 2 standard deviation: {within_3_std/100}%")
```
