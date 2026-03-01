---
{"dg-publish":true,"permalink":"/notes/poisson-distribution/","tags":["statistics","probability"]}
---

# poisson distributions
poisson distribution is a [[Notes/discrete probability distributions\|discrete probability distribution]] used to model the likelihood of a specific number of events occurring within a fixed interval of time or space.
this [[Notes/probability distributions\|distribution]] is particularly useful in scenarios where events happen [[Notes/independent events\|independently]] at a constant average rate and the probability of multiple occurrences within a short interval is low

its shape varies based on the frequency of events, ranging from right-skewed to approaching normal as occurrences become more frequent
![Pasted image 20250803201454.png](/img/user/Notes/Pasted%20image%2020250803201454.png)

the poisson distributions graph is right skewed (i.e. long tail on the right side) when the frequency of past occurrences is low, because the [[Notes/probability mass function\|PMF]] returns a distribution that estimates high probability for a small number of events and low or zero [[Notes/probability\|probabilities]] for a large number of [[Notes/event\|events]].
#### characteristics of poisson distributions
1. because poisson distributions are inherently discrete, they are used exclusively to model countable events.
2. this entails that only non-negative integers are applicable, as countable events cannot be negative.
3. these are typically _fixed within a predefined interval of time or space_, such as the number of arrivals within an hour, or the count of typographical errors per page.

#### applications of poisson distribution
it can model the annual occurrences of meteor showers, the diagnosis count of measles within a year, daily text message traffic, hourly customer purchases, accidents at a specific intersection during peak hours, or the hourly inbound call volume received by a customer service center.
