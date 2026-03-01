---
{"dg-publish":true,"permalink":"/notes/binomial-coefficient/","tags":["probability","statistics"]}
---

# binomial coefficient
it is a mathematical quantity that represents the number of ways to choose a specific number of items from a large set

it is often read as `n choose k`

the binomial coefficient is denoted in a few common ways, most notably:
$$
\binom{n}{k} \text{ or C(n,k)}
$$

it is calculated using the [[Notes/combinations without replacement\|combinations without replacement]] formula:

$$
\binom{n}{k} = C(n,k) = \frac{n!}{k!(n-k)!}
$$


It is done using without replacement formula, because once we got a trial as a success, we cannot include it again when choosing another success trial. We cannot use the __with replacement__ model, because an experiment is a sequence of distinct trials, and each trial happens only once.
