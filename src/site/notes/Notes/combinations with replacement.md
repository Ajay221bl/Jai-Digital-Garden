---
{"dg-publish":true,"permalink":"/notes/combinations-with-replacement/","tags":["combinatorics","probability"]}
---

# combinations with replacement

formula is derived from the [[Notes/combinations without replacement\|combinations without replacement]] formula.
 
when replacement is allowed, we still choose $r$ items from, a set of $n$ distinct items, but we allow any item to be selected multiple times. To then derive the formula for combinations with replacement, we'll introduce the concept of dummy items.
we add $r-1$ dummy items to the set before making selections. hence in the formula of [[Notes/combinations without replacement\|combinations without replacement]] which is :
$$
\frac{n!}{r!(n-r)!}
$$
we replace the $n$    with    $\text{n + (r-1)}$  because we have added dummy items which are one less in number than the r. so the new $n$ would be $n + (r-1)$ 

substituting value in the above formula:
$$
\frac{(n+(r-1))!}{r!((n+(r-1))-r)!} = \frac{(n+r-1)!}{r!(n-1)!}
$$

if $n$ equals $5$ available ingredients and $r$ equals $3$ total selections, the number of possible [[Notes/combinations with replacement\|combinations with replacement]] equals:
$$
\frac{5+3-1}{3!(5-1)!} = \frac{7!}{3!\times{4!}} = \frac{5040}{6\times{24}} = 35 \text{ possible combinations}
$$
