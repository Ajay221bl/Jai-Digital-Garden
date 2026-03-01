---
{"dg-publish":true,"permalink":"/notes/binomial-experiment/","tags":["statistics","probability"]}
---

# binomial experiment
a binomial experiment is a [[statistical experiment\|statistical experiment]] in which a [[Notes/binomial random variable\|binomial random variable]] represents the number of successes in a fixed number of repeatable trials, where the probability of success is consistent throughout.

the trials are [[Notes/independent events\|independent]] of each other
the outcome of each trial must be classifiable into one of two categories:
- heads or tails
- yes or no
- pass or fail
- defective or non defective



lets consider the classic example of flipping a fair coin 5 times and counting the number of heads. This is a binomial experiment because:
1. fixed number of repeated trials (5)
2. [[Notes/probability\|Notes/probability]] of success in each trial is constant (probability of getting a head is 0.5 in case of a fair coin in any number of trials)
3. [[Notes/independent\|independent]] trials (the outcome of one trial doesn't influence other trials)
4. two possible outcomes (each flip can either be heads("success") or tails("filure"))

when the above mentioned conditions (fixed number of trials, independent trials, two possible outcomes, constant probability of success) are met, the [[Notes/binomial distribution\|binomial distribution]] can be used to calculate the [[Notes/probability\|Notes/probability]] of getting a certain number of successes in a fixed number of trials
