---
{"dg-publish":true,"permalink":"/notes/logistic-function/","tags":["statistics","probability"]}
---

# logistic function $\sigma(x)$

The function transforms the linear combination of the [[Notes/explanatory variables\|predictors]] into a [[Notes/probability\|Notes/probability]] for each record in the data that equals some value between $\text{0 and 1}$. When the [[Notes/probability\|Notes/probability]] equals $\text{50\%}$ or greater, the model is predicting the binary outcome to equal 1; conversely, when the [[Notes/probability\|Notes/probability]] is less than $\text{ 50\%}$, the model is instead predicting the binary outcome to equal $0$.

The sigmoid function is typically written in its standard form as:
$$
\sigma(x) = \frac{1}{1+e^{-x}}
$$
when the input $x$ is large, either positive or negative, the value of $e^{-x}$ approaches $0$, causing the [[Notes/sample space\|denominator]] of the fraction to become large, thereby resulting in $\sigma(x)$ being close to 1. Conversely, when $x$ is large in the negative direction, $e^{-x}$ subsequently becomes large, causing $\sigma(x)$ to approach $0$.

![Pasted image 20250818184629.png|500](/img/user/Notes/Pasted%20image%2020250818184629.png)


We get [[Notes/probability\|probabilities]] by plugging the [[Notes/explanatory variables\|predictors]] and their coefficient into this [[Notes/logistic function\|sigmoid function]], where the input is replaced by a linear combination of [[Notes/explanatory variables\|predictor]].
$$
\large\text{P(Y=1|X)}= \frac{1}{1 + e^{-(\beta_{0}+ \beta_{1}X_{1}+\beta_{2}X_{2}+ \beta_{3}X_{3})}}
$$
where
- $P(Y=1|X)$ is the [[Notes/probability\|Notes/probability]] of the outcome variable, designated as $Y$, being 1 given the predictor variable $X$.
- $e$ is the base of the [[natural logarithm\|natural logarithm]], equal to $2.72$.
- $\beta_{0}$ is the intercept term.
- $\beta_{1}$, $\beta_{2}$ and $\beta_{3}$ are the coefficients of the [[Notes/explanatory variables\|predictor]] variables.
- $X_{1}$, $X_{2}$ and $X_{3}$ are the [[Notes/explanatory variables\|predictor]] variables
